
# Bash cheat sheet

change extension:
for f in *.info; do  mv -- "$f" "${f%.info}.txt"; done

Excel
=AND(NOT(ISBLANK(C2));RIGHT(TRIM(C2);2)<>".0";C2<>"N/A";C2<>"ver.")
=AND(NOT(ISBLANK(E1));RIGHT(TRIM(E1);2)<>".0";E1<>"N/A";E1<>"ver.";E1<>"Column4";D1<>"Supplier Register")

----------------------------

# New employee
- Jira, Slack, GitHub, Ahjo, Drobpox, Sharepoint, Microsoft

----------------------------

# Sampo Documentation
https://www.dropbox.com/work/Sampo/Marketing%20materials/Customer%20data%20sheet
https://www.dropbox.com/work/Maxim/Sampo%20documents

# Customer share folder
Aino1:
https://www.dropbox.com/sh/uvapw499s6yjdba/AACzbhdoJoQ5m6fjwKQKBFoUa?dl=0
Sampo:
https://www.dropbox.com/sh/82t1anyp4c67x1p/AADBtMv3J_b6QQsVvnq34oCla?dl=0
SampoMaxim:
https://www.dropbox.com/sh/iebp0uwlyu79hgg/AADAhC4PnxOWBVh5ZzzG47KXa?dl=0

# Sharepoint document link
https://pulseonfi.sharepoint.com/sites/medical
http://pulseonfi.sharepoint.com/_layouts/DocIdRedir.aspx?ID=PODMS-782466528-122
https://pulseonfi.sharepoint.com/projects/_layouts/15/DocIdRedir.aspx?sourcedoc=PODMS-782466528-122&action=read

https://docs.matrixreq.com/faq/how-to-avoid-browser-filling-my-user-name-in-input-fields/

----------------------------

# AFE control
- 2*R_2*(f)/1.2*(A_1*1.2/(2*(f)*R_1)-I_c*1e-6)
- 2*R_2*f/1.2*(A_1*1.2/(2*f*R_1))
- https://www.wolframalpha.com/input/?i=2*R_2*%28f%29%2F1.2*%28A_1*1.2%2F%282*%28f%29*R_1%29-I_c*1e-6%29

- TI_AFE4950 configuration tool == compiler "downstream" qualification

AGC tallennus: RnD tai Debug softa ja PPG raw oltava päällä

----------------------------

# Ambulatory
N7Wn59R45QYsAPoSMPzGiPEycd86Diw9XMEDawFdCeX7X3Z6A5Rgu8Dr
ssh -p 19092 -i some.key pulseon@localhost

----------------------------

# Hardware

ADC_RDY menee MCU:lle
GPIO2 menee ACC:lle

päällä: RLD, INM
pohjalla: INP

## Markon laitteet
AEP41,  HW revision: 1.0
AEP57,  HW revision: 1.1
AEP77,  HW revision: 1.2
000065, HW revision: 1.3
000102, HW revision: 1.3.1

---------------------------

# Links

AWS login:
https://pulseon-test.signin.aws.amazon.com/console
https://pulseon-prod.signin.aws.amazon.com/console


# GitHub Repos

https://github.com/PulseOn/Orchestration
https://github.com/PulseOn/Cardiolund-Ms
https://github.com/PulseOn/dms
https://github.com/PulseOn/dmsdatabase
https://github.com/PulseOn/ims
https://github.com/PulseOn/nginx
https://github.com/PulseOn/pdf-service
https://github.com/PulseOn/wds
https://github.com/PulseOn/atostek

https://github.com/PulseOn/Automated-tests
https://github.com/PulseOn/dts

https://github.com/PulseOn/WebRenderer

# DMS IMS

Device API https://localhost:5001/api/device/versioninformation
https://ims.test.pulseon-ecg.com/Devices/DeviceList?deviceUid=00112233445566778899AABBCCDD

---------------------------

# Battery life

Old battery in reflector test
7 days and 5 hours
7 days and 6 hours
7 days and 4 hours

New battery with SW fuel gauge in reflector test
6 days 12:56:03
6 days 16:20:51
6 days 18:14:24
6 days 17:21:08

3.35 V sammutus = 
change critical from 8 -> 5
low from 12 -> 9

low 12%, critical 8%
pre-quiet time period: 3h
quiet time DMS default 22:00-08:00 (10h)
battery testing 100% -> 8%: 9d1h, 8d13h

------------------------------------
# Audit
- tool qualifications
- tool re-qualifications
- post-market surveillance
- sw development plans --> sw development
   --> update X-ray instructions

## List of GWs

https://pulseonfi.sharepoint.com/sites/medical/Projects/Aino%20ECG/Design%20Deliverables/Design%20Transfer/Builds/HWP4/Aino%20ECG%20proto%20devices%20list%20and%20status.docx

## GW debugging

### Reinstall
ssh -i ~/.ssh/gw_key -p 32664 gwadmin@localhost "nohup sudo sh -c 'opkg remove pulseon-rssh && opkg remove pulseon-app && opkg remove \"pulseon-dms-config-*\" && shutdown -r now' > /dev/null 2>&1 &"

# Reinstall and restart pulseon-reinstaller
~/debugging/update_gw_fw_mn.sh -b ~/gw-bundles/GW-237-FW-7.3.2/artifacts/pulseon-gateway_prod-dna-eu_1.0.13~8~gdaa3102.tar.gz -r ~/gw-bundles/latest/pulseon-reinstall_1.0.13.ipk -v 7.2.3 -w -p 44706
~/test/gw_pulseon-bundle_install.sh -p 32664 -R -r /root/gw-bundles/PR-95-nr18/pulseon-reinstall_1.0.7~17~g9581cdab2c.ipk /root/gw-bundles/PR-95-nr18/pulseon-gateway_test-dna-eu_1.0.7~17~g9581cdab2c.tar.gz
~/debugging/run_in_screen.sh '~/gw-scripts/gw_pulseon-bundle_install.sh -p 36754 -f -R -r /root/gw-bundles/FW-7.3.2-fixbands-PR-147_nr2/pulseon-reinstall_1.0.13~11~g12f82e04a84.ipk /root/gw-bundles/FW-7.3.2-fixbands-PR-147_nr2/pulseon-gateway_prod-monogoto-eu_1.0.13~11~g12f82e04a84.tar.gz'
ssh -i ~/.ssh/gw_key -p 32664 gwadmin@localhost "nohup sudo systemctl restart pulseon-reinstaller > /dev/null 2>&1 &"

opkg remove pulseon-rssh && opkg remove pulseon-app && opkg remove "pulseon-dms-config-*"
opkg remove --force-remove pulseon-rssh && opkg remove --force-remove pulseon-app && opkg remove --force-remove "pulseon-dms-config-*"
fix opkg status
/var/lib/opkg/status
/usr/sbin/pulseon-reinstall
/mnt/data/etc/updatehooks.user.d
/mnt/data/opt/pulseon-app/pulseon-gateway-latest.tar.gz
grep -vE "^#|^$" /opt/nbiot_connection/modem.cfg

systemctl list-unit-files | grep pulseon
sudo opkg install /home/gwadmin/pulseon-reinstall-latest.ipk --force-overwrite

rm -rf /mnt/data/opt/pulseon-app/pulseon-gateway-latest.tar.gz
rm -rf /mnt/data/etc/updatehooks.user.d/*


rm /usr/share/ca-certificates/mozilla/DST_Root_CA_X3.crt && sed -i '/DST_Root_CA_X3.crt/d' /etc/ca-certificates.conf && update-ca-certificates
sudo curl --insecure --cert /mnt/identity/device_cert.pem --key /mnt/identity/device_key.pem https://debug.treon.fi/patches/DST-X3-cert-removal.44046e99.202110061015.sh > /tmp/patch.sh && sudo bash /tmp/patch.sh
nohup sudo su -c 'fwupdate-run --use-device-cert https://debug.treon.fi/treongw1-v7.2.0.20231219091313/treongw-image-iotgw_7.2.0.20231219091313.tar' > fwupdate_$(date -I).log 2>&1 &
FW 7.1.1
GW1: fwupdate-run --use-device-cert https://debug.treon.fi/treongw1-v7.1.1.20230612080149/treongw-image-iotgw_7.1.1.20230612080149.tar
GW2: fwupdate-run --use-device-cert https://debug.treon.fi/treongw2-v7.1.1.20230612092222/treongw-image-iotgw_7.1.1.20230612092222.tar
FW 7.2.0
GW1: fwupdate-run --use-device-cert https://debug.treon.fi/treongw1-v7.2.0.20231219091313/treongw-image-iotgw_7.2.0.20231219091313.tar
GW2 (unreleased): fwupdate-run --use-device-cert https://debug.treon.fi/testimages/jenkins/rel/7_2_0/21/treongw2/treongw-image-iotgw_7.2.0.20231219104440.tar

## Logs

grep -E "WARNING|ERROR|Downloading|Succesfully" journal.log
~/debugging/run_for_each_gw.sh -s -u 44696 -u 32664 'sudo journalctl -u pulseon-app -S today'
~/debugging/run_for_each_gw.sh -s -u 44677 -u 45651 -u 36754 -u 44706 -u 44600 -u 44688 -u 32711 -u 32767 -u 44696 -u 32664 'sudo journalctl --boot -u pulseon-app grep -E "WARNING|ERROR|Downloading|Succesfully"'

### Other

btmgmt find -l
systemctl restart pulseon-app
systemctl status "pulseon*"
journalctl -u pulseon-app -S today
journalctl -u pulseon-app -f
journalctl --boot --lines=all | gzip -c > $HOSTNAME-journal-$(date +%Y.%m.%dT%H.%M).log.gz
cat /etc/machine-id
sudo find /mnt/data/var/log/journal/ -mindepth 1 ! -name $(cat /etc/machine-id) -type d -exec rm -rf {} +
chown -R gwadmin:gwadmin /home/gwadmin/

bluetoothctl
scan on
menu scan
clear
transport le

### Updating
~/debugging/run_in_screen.sh '/root/debugging/update_gw_fw_mn.sh -w -r ~/gw-bundles/latest/pulseon-reinstall_1.0.13.ipk -v 7.3.2 -b /root/gw-bundles/FW-7.3.2-fixbands-PR-147_nr2/pulseon-gateway_test-twilio-eu_1.0.13~11~g12f82e04a84.tar.gz -p 32637'
~/debugging/run_in_screen.sh '/root/debugging/update_gw_fw_mn.sh -l -r ~/gw-bundles/latest/pulseon-reinstall_1.0.13.ipk -v 7.3.2 -b /root/gw-bundles/FW-7.3.2-fixbands-PR-147_nr2/pulseon-gateway_prod-dna-eu_1.0.13~11~g12f82e04a84.tar.gz -p 32711'

### Changing services
/lib/systemd/system/ofono.service: /usr/sbin/ofonod -n > /usr/sbin/ofonod -n -d
/opt/nbiot_connection/config_modem.sh: config_modem.py; > config_modem.py -l DEBUG;
sed -i 's/config_modem.py;/config_modem.py -l DEBUG;/g' /opt/nbiot_connection/config_modem.sh
vim /lib/systemd/system/ofono.service
vim /lib/systemd/system/bluetooth.service
systemctl daemon-reload

### cellular
connmanctl technologies
/usr/lib/ofono/test/list-modems
python /opt/nbiot_connection/ofono_control.py -v -w --scan
dbus-send --system --print-reply --dest=org.ofono /ubloxmodem_0 org.ofono.NetworkRegistration.GetProperties
cat /var/gw-system-manager/reset_reason

#### more logging on cellular
c
sed -i 's/MODEM_URAT="7,9"/MODEM_URAT="7"/g' /opt/pulseon-app/config/opt/nbiot_connection/modem.cfg
sed -i 's/MODEM_URAT="7,9"/MODEM_URAT="7"/g' /opt/nbiot_connection/modem.cfg


In case of config change:
cd /opt/nbiot_connection/
systemctl stop nbiot
systemctl stop ofono
python3 config_modem.py -l DEBUG
systemctl start nbiot


### copy files
rsync -az --progress -e 'ssh -i ~/.ssh/gw_key' --rsync-path="sudo rsync" --include='*.log.gz' --exclude='*' gwadmin@treongw1-d8f4cacb.:/home/root/ .
rsync -az --progress -e 'ssh -i ~/.ssh/gw_key' --rsync-path="sudo rsync" --include='*.log.gz' --exclude='*' --remove-source-files gwadmin@treongw1-fe76b6e7.:/home/root/ .
rsync -az --progress -e 'ssh -i /root/.ssh/gw_key -p <port-number>' --rsync-path="sudo rsync" --include='*.log.gz' --exclude='*' gwadmin@localhost:/home/root/
rsync -azv --rsync-path="~/rsync" --include='*.py' --exclude='*' . ahjo.pulseon.fi:cardiolund/pulseon_demo_system/
# Copy a list of files
rsync -azv -m --rsync-path="~/rsync" --info=progress2 --include-from=files.list --exclude='*.csv' ahjo.pulseon.fi:/opt/clinical_study/pulseon_demo_system/patientData_export_UIDS/ ecg_filter_poorq_pulseon_demo_system
```files.list
*/*/2023-08-29T08.11.15.168+00.00.csv
*/*/2023-08-27T18.04.24.817+00.00.csv
```

# Gatekeeper

~/debugging/run_for_each_gw.sh -s -u 44677 -u 45651 -u 36754 -u 32637 -u 44600 -u 44688 -u 32664 -u 44696 -u 32767 'sudo /usr/lib/ofono/test/list-modems && sudo journalctl --boot -u pulseon-app | grep -E "WARNING|ERROR|Downloading|Succe
sfully"'

ssh -C -i ~/.ssh/gw_key -p 32637 gwadmin@localhost "sudo journalctl -u pulseon-app | grep ':ERROR:' | awk -F ':ERROR:' '{print \$2}' | sort | uniq -c | sort -nr"
test/connected_gw_ports.sh | xargs -i test/gw_check_ethernet.sh -p {}
test/connected_gw_ports.sh | xargs -d $'\n' sh -c 'for arg do echo "GW $arg"; ssh -C -i ~/.ssh/gw_key -p 32637 gwadmin@localhost "sudo journalctl -u pulseon-app | grep \":ERROR:\" | awk -F \":ERROR:\" \"{print \$2}\" | sort | uniq -c | sort -nr"; done' _

PORT=32664; ssh -i ~/.ssh/gw_key -p $PORT gwadmin@localhost 'sudo journalctl -u pulseon-app --since "2023-08-11 14:10:00" | gzip -c' > ~/debugging/journal-$PORT.gz

# GW log analysis

## Concatenate multiple files with filename
tail -n +1 *.log
awk -F':ERROR:|:INFO:|:DEBUG:|:WARNING:' '{print $2}' journal-1e0293de-04-10_july.log | sort | uniq -c | sort -nr > unique_lines.txt
cat *.log | awk -F':ERROR:|:WARNING:' '{print $2}' | sort | uniq -c | sort -nr > warnings_errors

grep -E "systemd-networkd|gw_system_manager|pulseon-rssh|gw-ssh|context|ppp0" treongw1-6b4f546c-230905-0914.log

grep "RSSI" gw.log | sort -n -t '=' -k4 > gw_rssi.log
grep -E "Device = D7:10:60:EF:AC:CB|passkey: 707873|BLE pair error|Downloading File|files available" treongw1-600d9c1a-230905-1625.log

grep -Pazo "(?<=707873)[\s\S]*?(WARNING.*|Downloading File.*)\N" treongw1-600d9c1a-230905-1625.log

## GW characteristic writing method
- uses notifications
- WD 159 ble max packet size
   + effective size is 244

CONFIG_BT_BUF_ACL_RX_SIZE=251
CONFIG_BT_L2CAP_TX_MTU=247
CONFIG_BT_BUF_ACL_TX_SIZE=251
CONFIG_BT_CTLR_DATA_LENGTH_MAX=251


## Improvements
Suostuu aloittamaan session akulla, joka on tyhjempi kuin 98%.
Introduce waiting for release state in PULTEK project
- session aloittaessa ei avaa edes näkymää, jos on käynnissä oleva
- muuta päivän värjäysperuste: keltainen (fast/slow) punainen (arrhythmia)

# Windows 11 apps to install

- 30 pcs (some to Jari, some the Kyrel)

- AINO-DIR-052 regular security audit
- AINO-DIR-060 specify actual requirements

Tests
- https://pulseon.atlassian.net/browse/AIVER-145 never run
- https://pulseon.atlassian.net/browse/AIVER-149 could be linked to USB and BLE requirements 


# TODO

- device history file - do we need to specify the version
- Design plans and their version history as a result of design evolution.
- suggest bring back friday call with all company where malla presents stuff
- GW task for PULTEK-1186

- https://pulseon.atlassian.net/browse/PULTEK-1281 update to Feedback register #118
- https://pulseon.atlassian.net/browse/PULTEK-1280 update to Feedback register #110
- Update Service Admin Manual
- Update AMS-1 Security

## Periodic checks
- Automatic monitoring of audit logs
Add a periodic check for algorithm results.
- sanity check for periodic algorithm after some time.
- NTP fallback into periodic check list

------------------------

# --key=1,2 means take first two fields into account (separator is whitespace by default)
2023-10-24 05:41:12.752 (1698126072752): PULSEON_ALGORITHM_IBI IBI 521 0 1 0
_______________________
cat actana_parsed.log app_events_parsed.log messages_parsed.log | sort --stable --key=1,2 > all_parsed.log
cat *.log | sort --stable --key=1,2 > all_parsed.log

----------

View recommendations
https://entra.microsoft.com/?culture=en-us&country=us#home

----------

Clinical (ambulatory) study
434 ECGs uploaded to IMS
- all 434 bad quality by ECG filter
- 332 non-sinus non-poorq
- DMS shows 6 as good quality (sinus)

---------------

UK NHS DTAC
ORCHA certification to help with DTACH
DCP 0160

---------------

Use old approved form.
Concerns on new template.
URS approval in Jira.

---------------

settingsclient.py -s com6 -i 1 -w 0x62; settingsclient.py -s com6 -i 3 -w 1; settingsclient.py -s com6 -i 5 -w 0; ftsclient.py -s com6 --delete-really;

--------------

TODO
PULTEK: Priorisoi sairaalalogo, FHIR
Sydänkeskus external and internal doctor

Confirm: cytotoxicity

Confirm softa kuntoon with Jari
Go though backlog

double-check https://pulseon.atlassian.net/browse/OHRSW-2334

Task for GW USB data transfer

------------

GW release in 2 weeks.
GW FW upgrade remotely.
DIR for FHIR integration
Add a risk for file upload virus
------------
Synlab 2024-09-17:
- kuka lääkäri on lausunut ja montako mittausta ja missä tomipisteessä?
- laskutusperuste: kuka annotoi, eikä merkitse valmiiksi
- raporttiin kuka lausui (ja bonuksena alkuperäinen hoitava lääkäri)
- copy/paste liitä määräten ottaa taulukosta
- hoitajan valinta: skannaako tiedostona (jpg ja pdf) vai kirjoittaako
  - Koko tallennuksen aikainen päiväkirja (yksi yksittäinen kenttä)

- loppuepikriisi
-----------
Idoven 2024-09-17
- https://en.wikipedia.org/wiki/HL7_aECG, no context in that message
- Coming HL7 FHIR
- Willem Workspace to visualize data


----------------

https://security.microsoft.com/reportsubmission?viewid=email&tid=cc630003-2761-4b58-9e69-63a9d16eb094
https://security.microsoft.com/tenantAllowBlockList?tid=cc630003-2761-4b58-9e69-63a9d16eb094


collapsipotilas: pyörtyy -> pitkät tauot: RR väli yli 4 sec 5 sec



Balazs:
- USB data transfer of GW
- feature to not transfer files to DMS just keep locally
- Balazs: test transient error alarm in IMS once https://pulseon.atlassian.net/browse/OHRSW-2399 is done

Atostek:
- release target on 24-25
- risk management update today


TODAY:
- [GW-250](https://pulseon.atlassian.net/browse/GW-250) pull request use treon settings
- 01.00.15 approvals
  - immediate action minutes
- Software safety classification justification (see email)
- Jira re-qualification
- Record file index jump steps to reproduce
- PROD DB
  - Device SMQ events - fetch discharge curves from IMS DB
  - 000243 22.9.2024 -> today
  - Jari battery low started too soon: Device 000820 start 2024-09-27
  - Ari: battery low started in prod after 2 days: UDI 000243, start 2024-09-22 - today
  - Jaakko: low battery started too soon: Device 000773, alert start evening of 2024-10-22
  - AMS1OPS devices
- c_term update for Tuomas
- Kuluttajariitalautakunta
- Remonttiraportti
- Add HL7 as DIR
- email läppärin hankinnasta Jari Jaakko
- Confirm fuel gauge charging issue with Jari. More picky about charging with UI indication.
- Markun laite (01)06430054330121(10)0222(11)220118(21)000213
