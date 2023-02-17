Connect with J-Link
```
JLinkExe -device nRF52840_xxAA -if swd -speed 4000 -AutoConnect 1
```
NOTE: You may get a popup at this point asking to unsecure the device. Select Yes two times if asked.

Erase
```
erase
loadbin _zero_ram.bin, 0x20000000
```

Flash
```
loadfile AinoEKG-0.7-Release.hex
exit
```

The macroboard should start up at this point.

###############################

```cfg
# Set modem Radio Access Technology priorities
# 7: LTE Cat M1
# 8: LTE Cat NB1
# 9: GPRS
# Allowed values for Sara 410M: 7,8 and 412M: 7,8,9
# Maximum of three technologies can be set
MODEM_URAT="9,7,8"

# SIM pin code
PIN=""

# Set this if you wan't to override default APN
# Note that ofono saves this value once set
APN="nat.iot.dna.fi"

# Set this if authentication is required for APN
# Allowed values (none, chap, pap)
AUTHENTICATION="none"
APN_USERNAME=""
APN_PASSWORD=""

# Allow roaming
ROAMING="true"

# For certain networks UMNOPROF needs to be set properly. In most cases this
# should not be modified as by default UMNOPROF="100"
# settings based on SIM card. However, if setting APN fails one can try following
# different values for each operator listed:
# 0 - Modem SW default, all bands
# 1 - Detect from sim card
# 2 - AT&T
# 5 - T-Mobile US
# 19 - Vodafone
# 31 - Deutsche Telekom
# 100 - Standard Europe
UMNOPROF="100"

# Manually selected network id
NETWORK=""

# Set lte bands, by default europe bands are used (3,8,20)
# Comma-separated list with allowed values 2, 3, 4, 5, 8, 12, 13, 20, 26, 28
LTE_BANDS=""
```

Sep 27 12:23:52 treongw1-aae07875 python3[278]: 2022-09-27 12:23:52:INFO:Connected to device: PulseOn AM-1
Sep 27 12:23:53 treongw1-aae07875 python3[278]: 2022-09-27 12:23:53:WARNING:D-Bus call failed: org.bluez.Error.Failed: Operation failed with ATT error: 0x0e
Sep 27 12:24:29 treongw1-aae07875 systemd-journald[120]: Forwarding to syslog missed 8 messages.
Sep 27 12:24:57 treongw1-aae07875 python3[278]: 2022-09-27 12:24:57:WARNING:We did not get all the data!


btmgmt find -l

python /opt/nbiot_connection/ofono_control.py --list-networks