
# Instructions

### Settings

| Setting ID | Name | Values |
|-|-|-|
| 0 | AINO2_SETTING_AF_NOTIFICATIONS_ENABLED | 0 = disable, 1 = enable |
| 1 | AINO2_SETTING_RECORDING_SOURCES_ON_HAND | Bitmask (see blow) |
| 2 | AINO2_SETTING_RECORDING_SOURCES_AF | Bitmask (see blow) |
| 3 | AINO2_SETTING_FORCE_WORN_STATE | 0 = off hand, 1 = on hand |
| 4 | AINO2_SETTING_QUIET_TIME | timestamp |
| 5 | AINO2_SETTING_SHELF_MODE_ENABLED | 0 = disable, 1 = enable |
| 7 | AINO2_SETTING_ALERT_LOGIC_ENABLED | 0 = disable, 1 = enable |

### Recording sources for settings 1 and 2

| Source name | Source ID |
|-|-|
| ACTANA_SOURCE_ACCELEROMETER | 1 |
| ACTANA_SOURCE_PPG | 2 |
| ACTANA_SOURCE_PROXIMITY | 3 |
| ACTANA_SOURCE_ECG | 4 |
| ACTANA_SOURCE_ECG_LEAD_OFF | 5 |
| ACTANA_SOURCE_HAND_DETECTION | 6 |
| ACTANA_SOURCE_PULSEON_ALGORITHM_ARRHYTHMIA_DETECTION | 17 |
| ACTANA_SOURCE_PULSEON_ALGORITHM_IBI | 18 |
| ACTANA_SOURCE_PULSEON_ALGORITHM_ACTIVITY | 19 |

The sources are bit indexes. Multiple sources can be selected by providing a mask. For example selecting recording sources proximity + ECG means `1 << 3 (proximity) | 1 << 4 (ECG) = 0x18`

### One example of recording  

`settingsclient.py -s -i 1 -w 0x18` # Select proximity and ECG for on hand recording sources
`settingsclient.py -s -i 3 -w 1` # Force on hand
`settingsclient.py -s -i 5 -w 0` # Disable shelf mode
`settingsclient.py -s -i 7 -w 0` # Disable alert logic
