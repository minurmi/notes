
# PulseOn HW test result interpretation

## Parsing the logs

**For PCBA test number 15**

The log from the J-Link Segger RTT doesn't need to be parsed.

**For assembled devices test number 16**

1. Take the original log file and select all 59 characters long strings that follow the text
   `"value: (0x) `. Example looks like `13-54-65-73-74-20-31-34-3A-20-00-00-00-00-00-00-00-00-00-00`
2. Pick all the the entries that don't start with `02`  and convert them to ASCII text using for example
   an online tool found by searching "hex to ascii" in Baidu.
   From `Log 2018-03-28 15/37/49.txt` the parsed output looks like:
```
Test 14: Test 14 Started: PulseON Init Test: Putest thread start
Init Passedaccelerometer: OPERATIONALometer: OPERAFE: OPERATIONAL
proximity sensor: OPERATIONALsensor: OTest 14 Ended: PulseON Init
Test: PulsTest 16: Test 16 Started: PulseON Assembled TestseON
Assembled Tesrequesting test modeequesting test modwaiting for test
resultsng for test reOther Event: (13)Other
Event: (12)4;0;43790;0;0;0;1565751;4448;2096918;1700190
48;2096918;1got update, individual tests:
individ2;0;43898;124;0;1862;1142;42;3571
;1862;1;43898;124;1;5004;3432;126;99
1;5002;2;43898;124;2;3616;3361;56;30
;2;3612;3;43898;124;3;394
```

## Interpreting the log

Format of AFE output:
```
4;<index>;<time_ms>;0;0;0;<green_led>;<ambient>;<ir_led>;<orange_led>

```

From `Log 2018-03-28 15/37/49.txt` this looks like
```
4;0;43790;0;0;0;1565751;4448;2096918;1700190
```

Format of proximity output:
```
2;<index>;<time_ms>;<ignore>;<sensor_id>;<useful>;<avg>;<diff>;<offset>
```

From `Log 2018-03-28 15/37/49.txt` this looks like
```
2;0;43898;124;0;1862;1142;42;3571
2;1;43898;124;1;5004;3432;126;99
2;2;43898;124;2;3616;3361;56;30
2;3;43898;124;3;394
```

Notice that the `sensor_id` 3 ends too soon and the important `offset` reading is missing.

## Limit values

**Assembled devices AFE limits**

|     |  Green  | Ambient |    IR   |  Orange |
|-----|---------|---------|---------|---------|
| Min |  100000 |  -30000 |  100000 |  100000 |
| Max | 2097151 |   30000 | 2097151 | 2097151 |

**PCBA AFE limits**

|     | Green  | Ambient |   IR   | Orange |
|-----|--------|---------|--------|--------|
| Min |  85000 |  -30000 | 400000 | 110000 |
| Max | 230000 |   30000 | 950000 | 280000 |

**Assembled devices proximity limits**

|     | Sensor 0 | Sensor 1 | Sensor 2 | Sensor 3 |
|-----|----------|----------|----------|----------|
| Min |     3003 |       76 |       24 |      141 |
| Max |     4505 |      115 |       36 |      212 |

**PCBA proximity limits**

|     | Sensor 0 | Sensor 1 | Sensor 2 | Sensor 3 |
|-----|----------|----------|----------|----------|
| Min |     3008 |       82 |       28 |      142 |
| Max |     4513 |      123 |       42 |      213 |
