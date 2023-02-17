
## PulseOn production line tests

This document describes the PulseOn production line tests at Fenda.
These tests cover all the sensors that include: accelerometer (LIS2DS12),
proximity sensor (SX9310) and AFE4404.

Several of the tests measure the signal level of the acceleration,
proximity and optical sensors. PulseOn needs access to all the logs
from each test run on the production line to be able to determine
proper pass/fail criteria for each sensor. Please provide all the
logs from every test to PulseOn.

## PulseOn init test
### Test name
`< RESPONSE >3:14:0:PulseON Init Test< /RESPONSE >`

### Test content
Initial test that tries to communicate with the accelerometer (LIS2DS12),
proximity sensor (SX9310) and AFE4404 over the I2C bus.

**NOTE:** This test **must be** run before any other PulseOn test.

### Pass/fail criteria
I2C communication succeeds with all sensors.
The OPERATIONAL/FAILED info for each sensor is shown in the DEBUG tags.

```
< DEBUG >14:Init Passed< /DEBUG >
< DEBUG >14:accelerometer: OPERATIONAL< /DEBUG >
< DEBUG >14:AFE: OPERATIONAL< /DEBUG >
< DEBUG >14:proximity sensor: OPERATIONAL< /DEBUG >
< DEBUG >14:Test 14 Ended: PulseON Init Test< /DEBUG >
```

### After test fail
Check which sensor failed using information inside the DEBUG tags.
Check that the sensor are undamaged and the I2C lines are in good condition.

## PulseOn PCBA test
### Test name
`< RESPONSE >3:15:0:PulseON PCBA Test< /RESPONSE >`

### Test content
Starts and measures signal from the accelerometer (LIS2DS12),
proximity sensor (SX9310) and AFE4404.

**NOTE:** This test should be run **only** in the Segger when testing
the PCBA board. It **must not** be run when testing the assembled device
over Bluetooth.

### Pass/fail criteria
The signal levels measured by each sensor are within limits defined by PulseOn.
The signal levels for the sensors shown in the DEBUG tags. This information
is crucial for PulseOn to diagnose the failing test.
The OPERATIONAL/FAILED info for each sensor is shown in the DEBUG tags.

```
< DEBUG >15:Test 15 Started: PulseON PCBA Test< /DEBUG >
< DEBUG >15:requesting test mode< /DEBUG >
< DEBUG >15:waiting for test results< /DEBUG >
< DEBUG >15:4;0;24679;0;0;0;0;0;0;0< /DEBUG >
< DEBUG >15:2;0;24808;0;0;5332;3752;114;3429< /DEBUG >
< DEBUG >15:2;1;24808;0;1;808;705;1;96< /DEBUG >
< DEBUG >15:2;2;24808;0;2;3796;3317;36;28< /DEBUG >
< DEBUG >15:2;3;24808;0;3;3424;2866;52;175< /DEBUG >
< DEBUG >15:Test Failed< /DEBUG >
< DEBUG >15:accelerometer: OPERATIONAL< /DEBUG >
< DEBUG >15:AFE: FAILED< /DEBUG >
< DEBUG >15:proximity sensor: OPERATIONAL< /DEBUG >
< DEBUG >15:Test 15 Ended: PulseON PCBA Test< /DEBUG >
```

### After test fail
Check which sensor failed using information inside the DEBUG tags.
Check that the sensor are undamaged and the I2C lines are in good condition.

## PulseOn Assembled test
### Test name
`< RESPONSE >3:16:0:PulseON Assembled Test< /RESPONSE >`

### Test content
Starts and measures signal from the accelerometer (LIS2DS12),
proximity sensor (SX9310) and AFE4404.

**NOTE:** This test should be run **only** using Bluetooth when testing
the Assembled device. It **must not** be run when testing the PCBA board
using the Segger.

### Pass/fail criteria
The signal levels measured by each sensor are within predetermined limits.
The signal levels for proximity sensor and AFE are shown in the DEBUG tags.
The OPERATIONAL/FAILED info for each sensor is shown in the DEBUG tags.

```
< DEBUG >15:Test 15 Started: PulseON PCBA Test< /DEBUG >
< DEBUG >15:requesting test mode< /DEBUG >
< DEBUG >15:waiting for test results< /DEBUG >
< DEBUG >15:4;0;24679;0;0;0;0;0;0;0< /DEBUG >
< DEBUG >15:2;0;24808;0;0;5332;3752;114;3429< /DEBUG >
< DEBUG >15:2;1;24808;0;1;808;705;1;96< /DEBUG >
< DEBUG >15:2;2;24808;0;2;3796;3317;36;28< /DEBUG >
< DEBUG >15:2;3;24808;0;3;3424;2866;52;175< /DEBUG >
< DEBUG >15:Test Failed< /DEBUG >
< DEBUG >15:accelerometer: OPERATIONAL< /DEBUG >
< DEBUG >15:AFE: FAILED< /DEBUG >
< DEBUG >15:proximity sensor: OPERATIONAL< /DEBUG >
< DEBUG >15:Test 15 Ended: PulseON PCBA Test< /DEBUG >
```

### After test fail
Check which sensor failed using information inside the DEBUG tags.
Check that the sensor are undamaged and the I2C lines are in good condition.

# Other PulseOn tests
### Test names:
```
< RESPONSE >3:17:0:PulseON Cont HR Mode Set< /RESPONSE >
< RESPONSE >3:18:0:PulseON Sampled HR Mode Set< /RESPONSE >
< RESPONSE >3:19:0:PulseON Cont ACC Mode Set< /RESPONSE >
```

### Test content
These test **must not** be run in the production line. They are meant
only for PulseOn internal testing.



