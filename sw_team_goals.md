
# Software team targets for the next 6 months

1. Support algorithm team
    - Support clinical studies and data collection needs
    - Prioritise bugs
    - Implement new features as requested to improve usability and stability
        + Add AFE data to be logged
2. Support sales
    - Answer customer questions
    - Implement new features and fix bugs as decided case-by-case
3. Aino 2 macroboard
    - A demo software of AinoZ features running on Aino 2 macroboard
        + New SW modules
            * nRF52840 + SDK 15
            * BLE stack with softdevice 6
            * Serial bus driver with SDK 15
            * AFE4410
            * LIS2DW
            * 1 Gbit QSPI flash
    - Verify Aino 2 hardware design with demo software
        + Powers
        + Chips and bus lines
        + RTC clock drift
        + New AFE + ACC synchronisation mechanism
5. Medical processes
    - Take medical processes into use in daily development
    - Validate tools: Github, GCC toolchains, FreeRTOS
    - Develop and document procedures
6. Test infrastructure
    - Set up automated test infrastructure
    - Install new server with verified configuration
    - Set up test workers and necessary hardware
    - Communicate the test HW needs to hardware team
7. Aino 2 medical software
    - Start developing Aino 2 demo to medical grade software
        + Build SW module-by-module with a design - verification cycle
        + Keep a working demo software with full functionality on the side
    - Prioritise Screening use case with BLE connectivity
        + Use own Android app as demo (not medical software)
        + Goal is to replace Android app with Zenicor device
8. Aino 2 prototype
    - Verify wrist held prototype functionality
        + Signal quality
        + Electrical interference
        + Mechanical fit
