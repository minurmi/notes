# Notes
2019 Jan 25

## Present
- Espoo: Adrian Constantin, Jukka Jalkanen, Marko Nurmi
- Over telco: Zoltan Nuyl

## Discussion
- Firmware image header should include a checksum and signing information
    + check if HW support for cryptographic algorithms
- It should be possible to update also the softdevice
- Generate functional diagrams of update: bootloader and normal image
- Generate diagrams of user update scenarios
- 1 MB reserved in the external flash for the update image
    + When to erase?
- Recovery functionality
    + Recovery feature is a separate part of the bootloader that
      is entered by a button press pattern when the bootloader
      is starting
    + Recover a device in case of error. Not used in normal workflow.
    + Contains only the functionality to upload a new image over USB (no BLE)
