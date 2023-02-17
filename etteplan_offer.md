

"ECG data platform" should be changed to "PPG data platform (PPGDP)"

1. PPG data platform API requirements
    - The deliverable should detail where a particular API requirement is involved in the PPGDP and device use.
    - We propose to identify the requirements for the following split:
        + Windows app <--> PPGDP
            * data from device via USB to cloud, applying monitoring settings from cloud to device, fetching firmware update from cloud and applying it to device
        + PPGDP <--> browser front-end
            * data from cloud to browser for visualization, device monitoring settings from browser to cloud for setting up the device
        + PPGDP <--> hospital system
            * matching patients to hospital systems, exporting patient summary to hospital system
        + PPGDP <--> ECG device platform
            * importing ECG data from 3rd party ECG platforms
2.  Windows app (“via USB) architecture, and its development plan with lead time & investment
    - Tasks 2 and 4 should be done hand-in-hand and together with the hospital IT expert. Architecture shouldn't be planned (task 2) prior to understanding constraints of the environment (task 4).
3. Provisioning of devices by clinical personnel
    - At least the following use steps should be considered:
        + Assign the device to the organization
            * Do we need some sub-groups (eg "ward 8", "hospital 2" etc)?
        + Assign the device to a patient and apply monitoring settings
        + Verify that the device has proper firmware or it needs to be updated
            * Update firmware
        + Get the device from the patient when the monitoring period ends and get the patient data from the device to the patient. Patient may provide additional info/notes about the  monitoring period, e.g. diary, etc..
        + Get device diagnostics data (logged errors etc.) from the device
        + Adding provision-specific notes by MD (e.g. to be used by other medical personnel). Does our system need to support/mirror these? How about other manually written records by other medical personnel (nurses etc.) as well?
        + Assign the device to the next patient.
    - How do you take a device out of use?
    - Can you report problems about device? Mark the device faulty/lost in the system --> get a replacement device.
4. Deployment of native Windows application in hospital IT environment
    - Possibility of obtaining authentication token from hospitals own log-in system to be used by the Windows app. This would likely be a hospital specific component - architecturally to be easily replaceable to support different systems.




Puhdistus?
- Ultraäänipesu
- Rannekkeen vaihto
- NFC lataus / langaton

# Laitteen käyttö
Tarvitaanko BLE-yhteyttä? Toimiiko vain NFC/USB?

Fleet management

Mistä tiedetään, että akku on tullut ikänsä loppuun?

Mitä ratkaisuja mietitään gatewaylle?

Voiko gatewayn poweroida USB-liittimestä?

Miten laite otetaan käyttöön?

Etteplanin kommentti:
- Tarvitaanko potilaalle motivointinäkymä?


Antille: onko kontaktia Tampereella?
- 30 min tapaaminen
- Sairaala IT kontakti

Onko Saksa hyvä
606 

IEC 62443-4-1:2018
IEC 62443-4-2:2019

# 20.02.2020

- Ehdoton vaatimus: ranneke on oltava vaihdettava
- TAYS: laitehankinnan vaatimukset, salaus









