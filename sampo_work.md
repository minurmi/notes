# Remaining Sampo work

- BT power optimization and operation logic cleanup
    + When to turn services on/off
        * i.e. HR profile on only in sport mode
    + What advertisement interval and other parameters to use at what time
        * i.e. high bandwidth for OTS if client supports that
        * Example: https://developer.polar.com/wiki/H6_and_H7_Heart_rate_sensors
- Implement missing parts of the Object Transfer Service
    + Requires changes to the BLE and possibly filesystem
- General power management
    + Profiling power consumption, find out what drains the most battery
        + Wrongly configured HW?
        + Suboptimally configured peripherals?
        + Unnecessary processor load
    + Taking PPI into use?
- Fault management, i.e. how to handle SW and HW fault situations
    + SW fault
        * Detect by watchdog or other mechanism
        * Recover from fault
    + HW fault
        * Log and recover
        * If unrecoverable/too frequent --> indicate to user
- Finalise the Device Control Service
    + Define missing characteristics
    + Implement control logic to "control thread". Might require slight refactoring
- Updating the firmware
    + Mechanism to enter DFU mode in device SW
    + Is updating bootloader/softdevice needed?
- Testing, how to guarantee robust software
    + More unit test coverage?
    + Additional functional testing involving HW?
    + Real user testing
    + Algorithm parameter accuracy validation
- Log sport event start and stop into memory
- Implement device off mode
    + Minimize battery consumption while keeping time and data
    + Enter off mode when battery level below threshold
- Calibrate battery level calculation
- Vibra buzz when mode changed
- Factory test software
    + Secure firmware flashing
    + Collect data: MAC address and sign the firmware for that
    + Test result logging


## Already worked on by Kii

### Android SDK/app
- Add unit/functional test cases?
- Implement missing parts of the Object Transfer Service
- Add Nordic's DFU library to Android app
- Reconstruct absolute time from recorded timestamps
- Implement missing characteristics of the Device Control Service
- Separate application and SDK
- XXX Use slide button instead of this toggle button for RAW On / Off to avoid accidental button press.
- Problems
    + XXX BluetoothLeGatt stops transferring files: https://github.com/PulseOn/PulseOn_Android_SDK/issues/4
    + XXX BluetoothLeGatt doesn't manage to send RAW start and stop commands: https://github.com/PulseOn/PulseOn_Android_SDK/issues/2
    + XXX BluetoothLeGatt RAW button not up-to-date: https://github.com/PulseOn/PulseOn_Android_SDK/issues/5
    + BluetoothLeGatt crashes: https://github.com/PulseOn/PulseOn_Android_SDK/issues/3
    + "Total Samples" and "Avg HR" shown in the UI don't make sense: https://github.com/PulseOn/PulseOn_Android_SDK/issues/6
### Filesystem
- Unit/functional testing
- Add missing filetypes
    + Firstbeat
    + IBI
    + Custom?
- Verify thread safety
- Filesystem crashes
    + If flash is not erased at startup and/or files are erased during operation