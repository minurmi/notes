# Commands
change extension:
for f in *.info; do  mv -- "$f" "${f%.info}.txt"; done

Excel
=AND(NOT(ISBLANK(C2));RIGHT(TRIM(C2);2)<>".0";C2<>"N/A";C2<>"ver.")
=AND(NOT(ISBLANK(E1));RIGHT(TRIM(E1);2)<>".0";E1<>"N/A";E1<>"ver.";E1<>"Column4";D1<>"Supplier Register")

```
bluetoothctl
scan on
menu scan
clear
transport le
```

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
# QMS

## Prosessikuvauksia
- Github
- SOUP-päivitys - (ks. Quality manual)
- Työkalujen päivitys (ks. Quality manual)

----------------------------

# AFE control
- 2*R_2*(f)/1.2*(A_1*1.2/(2*(f)*R_1)-I_c*1e-6)
- 2*R_2*f/1.2*(A_1*1.2/(2*f*R_1))
- https://www.wolframalpha.com/input/?i=2*R_2*%28f%29%2F1.2*%28A_1*1.2%2F%282*%28f%29*R_1%29-I_c*1e-6%29

- TI_AFE4950 configuration tool == compiler "downstream" qualification

AGC tallennus: RnD tai Debug softa ja PPG raw oltava päällä

----------------------------

# Kore
ssh -i ~/.ssh/gw_key gwadmin@treongw1-6b4f546c


# Ambulatory
N7Wn59R45QYsAPoSMPzGiPEycd86Diw9XMEDawFdCeX7X3Z6A5Rgu8Dr
ssh -p 19092 -i some.key pulseon@localhost

## treongw2 office LAN
ssh gwadmin@treongw1-aae07875.

## Marko
ssh gwadmin@treongw1-4b5833f0
ssh -C -i ~/.ssh/gw_key -p 32664 gwadmin@localhost
APWD: yd16vJB?4w*S)ifv

## Jaakko (no anymore)
ssh gwadmin@treongw1-f0e44d6a
ssh gwadmin@192.168.0.128
ssh -C -i ~/.ssh/gw_key -p 32637 gwadmin@localhost
APWD: Wbw4C(O[WEmgGOKt

]
## Jari
ssh gwadmin@treongw1-5a58679a
ssh -C -i ~/.ssh/gw_key -p 32721 gwadmin@localhost

]
## Jari (old)
ssh gwadmin@treongw1-e66f5c0c
ssh -C -i ~/.ssh/gw_key -p 32569 gwadmin@localhost
APWD: q-RVs[mwId!M4Wwt

]
## Antti
ssh gwadmin@treongw1-4f922b84
ssh -C -i ~/.ssh/gw_key -p 32563 gwadmin@localhost
APWD: 29!h5rEJuD?ps+oe

## Office / Jaakko
ssh gwadmin@treongw1-600d9c1a
ssh -C -i ~/.ssh/gw_key -p 32767 gwadmin@localhost
APWD: Jg!7WBj3NoRHwBAc

## CI in Office
ssh gwadmin@treongw1-7c917ecf
ssh -C -i ~/.ssh/gw_key -p 32652 gwadmin@localhost
APWD: Mn4CTTMfTYmy0lv1

## Jari K. (office old)
ssh gwadmin@treongw1-3c112afb
ssh -C -i ~/.ssh/gw_key -p 30961 gwadmin@localhost
APWD: FlKd+mBI)i(tN2R-

## Balazs
ssh gwadmin@treongw1-d090c506
ssh -C -p 30966 gwadmin@localhost
APWD: r)977B3epS#n52[X

##] Adrian
GWID:  ee3b7354
PORT:  32629
APWD:  Mf%he17VpZ)Nea[D

#]
#ssh -p 32627 gwadmin@localhost
#ssh gwadmin@treongw1-0731b1ca
#+(ImO%suF89&-Yzs

Office
gwadmin@treongw1-3c112afb
ssh -p 30961 gwadmin@localhost
GW ID (Serial): 3c112afb
Password User: qKqiG4D+t5egJ-l8
Password Admin: FlKd+mBI)i(tN2R-
Password WIFI_AP: 7d35746a

GW ID (Serial): d090c506
Password User: p9PJSG*A5b1wEo8o
Password Admin: r)977B3epS#n52[X
Password WIFI_AP: a6ff8dd1

#] Gatekeeper pub key
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAINLyb+p1j0GG0aQ1moISM+dNQY2RdBW1bNq+0k6Ulf6h gatekeeper1

----------------------------

# Laitteet
AEP41,  HW revision: 1.0
AEP57,  HW revision: 1.1
AEP77,  HW revision: 1.2
000065, HW revision: 1.3
000102, HW revision: 1.3.1

----------------------------

# Laptops
Ole's laptop: T470 i7-7550U 24GB of RAM

----------------------------

## Treon

What could be disable?
What do iotgw and gw-reverse-ssh do? They consume around 15 MB per month. How can we save data?
nginx, configui, iotgw, gw-reverse-ssh
Firewall rules? Disallow incoming connections.

5sec WLAN access point --> 30 sec: clearaa käyttäjälevyn
- system manager package

GW without WiFi
- List of serial numbers that don’t have WiFi
- It has to be possible to tell if GW has/hasn’t WiFi during runtime
- Repeat testing:
	- E2E system testing to transfer data during normal monitoring use
	- GW firmware upgrade is able to reinstall the PulseOn bundle
	- Maintenance connection to gatekeeper1 works
	- PulseOn package installation/removal/upgrade works
- Documentation that EMC/RF certificate is still valid.
	- Is the schematics changed? Is the chip removed but trances there? Could “loose end” radiate?

- Incidents
- Major vulnerability issues

---------------------------

# Algo development notes

- check test coverage
- make sure there is at leat one test that does regression testing using the whole algorithm
- put everything in git
- verify algorithm tools that are used to make decisions
- If development is made in matlab, and ported to c, we would like to have comparison testing between matlab and c code
- algorithms repository vs matlab repository: algorithms have code that could be used in 

---------------------------

# XRay reviews

All the planned test executions have been completed. The test plan covers the scope set in the PODMS-1378432600-918 Aino Design Verification Plan and the executed tests show that the applicable requirements are met.

Reviewed and approved. The test execution contains appropriate comments for execution evidence and any discrepancies between test specification.

# AFE4950

ADC_RDY menee MCU:lle
# GPIO2 menee ACC:lle

päällä: RLD, INM
pohjalla: INP

---------------------------

# AAMU

HUOM laskutusjärjestelmämuutokset!!
mittauksen pituus valittavissa viikon blokeissa, laskutus menee valitun pituuden mukaan
- PAT-2.43...PAT-2.46
- session ID from header. Should PulseOn try to implement?
- Mikä status uusien user guide tiedostojen uploadaamisessa?

https://pulseon.atlassian.net/wiki/spaces/P/pages/2894856193/Proposed+additional+tasks+2

# Rekry
- Academic Works 45/e tunti

--------------------------------

# Atostek

- https://pulseon.atlassian.net/browse/OHRSW-2124 Voiko debugata yhdessä simulaattorin tiedostojen lähetystä
- https://pulseon.atlassian.net/browse/OHRSW-2144 Samanaikainen FW update ratkennut. Vaatii DTS päivitystä
- DTS.UI lakkasi toimimasta. Auttaako PulseOn debuggaus?

DMS API to return the file index of the next file when upload succeeds

1. Task Managerista sulki ohjelma windows valikosta
2. Tarvitaan tietokone, kristian ja tarmo.koressaar@fujitsu.com

Device API https://localhost:5001/api/device/versioninformation

Tarve on pystyä muuttamaan simulaattoriversiota.
https://pulseon.atlassian.net/wiki/spaces/P/pages/1939374113/IMS+API
https://pulseon.atlassian.net/browse/PULTEK-617

AWS login:
https://pulseon-test.signin.aws.amazon.com/console
https://pulseon-prod.signin.aws.amazon.com/console


# Repos

https://github.com/PulseOn/ims
https://github.com/PulseOn/dms
https://github.com/PulseOn/Automated-tests
https://github.com/PulseOn/WebRenderer
https://github.com/PulseOn/dmsdatabase
https://github.com/PulseOn/Cardiolund-Ms
https://github.com/PulseOn/Orchestration
https://github.com/PulseOn/dts
https://github.com/PulseOn/wds
https://github.com/PulseOn/atostek
https://github.com/PulseOn/nginx

---------------------------

# Battery

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

LOW BATTERY

low 12%, critical 8%
pre-quiet time period: 3h
quiet time DMS default 22:00-08:00 (10h)
battery testing 100% -> 8%: 9d1h, 8d13h

klo 10-11

---------------------------

- Lisää Aino Project Planiin maininta, että menetelmiä sovelletaan myös maintenace vaiheessa

- Increase the UDI field legth from 50 to 64. Current UID is 44.
- Battery test where it can go empty

###############

Atostek aamu

- Check what data is logged
	- Improvement: Wrist device log improved: logged representation improved and data is logged on system message events
- Does patientData.csv include cardiolund?
- FLAGGING: New improvement: If time is lost. Start from previous timestamp instead of 1970.

- Leikkaa 2.0 sekuntia vaan, jos on täyspitkä eli yli 32s

######## TODO

Voidaanko niputtaa lokaalit DMS-osoitteet `*.pulseon-ecg.com` alle?
- olisiko parempi, että DMS generoi asennuspaketin lennosta
- vai olisiko osoite json konfiguraatio-tiedostossa, jonka sairaala asentaa kaikille jälkeenpäin ja ajaa testauksen?

- Automaattinen tunnistus SIM kortista ja lataa sen mukaan oikea konfiguraatio

1. Ahjo board broke - near the wall - physically larger machine - swap it with board on vasara
4 mittausta menemään: austraia, baltmedika (latvia), sveitsi ja itävalta

Kuismalle tekstiviest allekirjoita toolchain qualification


Lisää patient listaan näkyviin ID
- extract processes from current plans into own procedure documents
- Define processes on reacting to serious incidents
- Check SW development procedure to have Xray review flow

62304 software katso mitä sanotaan Risk Management File
- SW development plan: Double check the SOUP component monitoring
- https://pulseon.atlassian.net/browse/OHRSW-2082
- https://pulseon.atlassian.net/browse/OHRSW-2065
- https://pulseon.atlassian.net/browse/OHRSW-1996
- https://pulseon.atlassian.net/browse/BUGS-39


# Sprint planning
- Remind Treon about the gw-system-manager package. Test it myself
- determine which GW was used with which device?

Run test run after production deployment
- check if there are duplicate tasks
- Admin: searching for users. Seeing user roles and _status_.



# DMS/IMS parannuksia
- session aloittaessa ei avaa edes näkymää, jos on käynnissä oleva
- Rename session info Start, Estimated end, Actual end.
- IMS multiple selection don't show tick-box if it's not tickable
- Have the ability to assing a device to system. Not only organization.
- Possibility to upload multiple
- Raportti laitteista, joita ei ole käytetty
- Atostek: palauta archive, menee listassa alimmaksi
BUGI: User should not be able to start a session without closing the previous one
- muuta päivän värjäysperuste: keltainen (fast/slow) punainen (arrhythmia)

# Johdon katselmointi
- Critial: vaikuttaa turvallisuuteen (potilas tai tietoturva) tai kliiniseen suorituskykyyn
- Tehtävä: Harjoittele kriittistä palveluutosta (1 viikko). Pyydä Atostekilta hahmotelma nopeasta muutoksesta.

# Processes
- have a process to and leave a trail of employee accounts


######################

Should we have a risk management team meeting
3.2. impacts on risks the change has risk impacts

###########

attach IBI data if it has arrhythmia state
ibi, sqe, ibi rhythm class, ectopic
ask Tuomas


##########
Audit
- tool qualifications
- tool re-qualifications
- post-market surveillance
- sw development plans --> sw development
   --> update X-ray instructions

###########

Not passed in tester: d2fc969d

GW debugging

Greece:
92eee5bd / 8935806181021053882 - 32613
7471bfb9 / 8935806181021054336 - 32602
9fff5f6a / 8935806181021053908 - 32684

Sweded:
ec66f676 - 32645

Japan:
1ab11473 - 32635

Spain:
Jari K -- Last connected: Jun  6 13:26:33 gatekeeper1 gw-ssh: Gateway connected: treongw1-f0e44d6a Port: 32637 RELEASE_VERSION = 6.2.0.20210705122932 pulseon-app - 1.0.1 pulseon-dms-config - 1.0.1 pulseon-rssh - 1.0.1
treongw1-600d9c1a connected 119 times
Jaakko -- Last connected: Aug 26 11:56:42 gatekeeper1 gw-ssh: Gateway connected: treongw1-600d9c1a Port: 32767 RELEASE_VERSION = 6.2.0.20210705122932 pulseon-app - 1.0.2 pulseon-dms-config - 1.0.2 pulseon-rssh - 1.0.2
treongw1-d090c506 connected 21 times

Italy:
ab9108de 36728

KORE
office 1 (markon pöydällä): treongw1-6b4f546c
ssh -i ~/.ssh/gw_key gwadmin@treongw1-6b4f546c.
ssh -i ~/.ssh/gw_key -p 32711 gwadmin@localhost

Jaakolle Ruotsiin:
Jarin pöydällä treongw1-5a58679a
ssh -i ~/.ssh/gw_key gwadmin@treongw1-5a58679a. 'sudo dbus-send --system --print-reply --dest=org.ofono /ubloxmodem_0 org.ofono.NetworkRegistration.GetProperties'
ssh -i ~/.ssh/gw_key -p 32721 gwadmin@localhost

Ihan uusi suoraan tehtaalta
ssh -i ~/.ssh/gw_key gwadmin@treongw1-66d50911.
ssh -i ~/.ssh/gw_key -p 32558 gwadmin@localhost
root@gatekeeper1:~# grep 66d50911 /var/log/messages
Sep 21 09:30:20 gatekeeper1 gw-ssh: Gateway connected: treongw1-66d50911 Port: 32558 RELEASE_VERSION = 6.2.0.20210705122932 pulseon-app - 1.0.3 pulseon-dms-config-prod-dna-eu - 1.0.3 pulseon-rssh - 1.0.3
Sep 21 09:51:18 gatekeeper1 gw-ssh: Gateway connected: treongw1-66d50911 Port: 32558 RELEASE_VERSION = 6.2.0.20210705122932 pulseon-app - 1.0.3 pulseon-dms-config-prod-dna-eu - 1.0.3 pulseon-rssh - 1.0.3
Sep 22 06:36:01 gatekeeper1 gw-ssh: Gateway connected: treongw1-66d50911 Port: 32558 RELEASE_VERSION = 6.2.0.20210705122932 pulseon-app - 1.0.3 pulseon-dms-config-prod-dna-eu - 1.0.3 pulseon-rssh - 1.0.3

## DMS tricks

https://ims.test.pulseon-ecg.com/Devices/DeviceList?deviceUid=00112233445566778899AABBCCDD

## List of GWs

https://pulseonfi.sharepoint.com/sites/medical/Projects/Aino%20ECG/Design%20Deliverables/Design%20Transfer/Builds/HWP4/Aino%20ECG%20proto%20devices%20list%20and%20status.docx

## GW debugging


btmgmt find -l
systemctl restart pulseon-app
systemctl status "pulseon*"
journalctl -u pulseon-app -S today
journalctl -u pulseon-app -f
journalctl -u pulseon-app | gzip -c > ${HOSTNAME}_pulseon-app_$(date -I's').log.gz
connmanctl technologies
bluetoothctl
chown -R gwadmin:gwadmin /home/gwadmin/
vim /lib/systemd/system/ofono.service
vim /lib/systemd/system/bluetooth.service
/usr/lib/ofono/test/list-modems
python /opt/nbiot_connection/ofono_control.py -v -w --scan

dbus-send --system --print-reply --dest=org.ofono /ubloxmodem_0 org.ofono.NetworkRegistration.GetProperties

PORT=32664; ~/gw-scripts/update_gw_fw_6x_to_6.5.1.sh -p ${PORT} -b ~/gw-bundles/gateway-1.0.5/pulseon-gateway_prod-dna-eu_1.0.5.tar.gz 2>&1 | tr -d '\r' | tee -a ~/gw-logs/treongw1-${PORT}_update_gw_fw_6x_to_6.5.1-$(date -I).log

Download 32.1KB/s

#####
ab9108de	352373197141323	scNGz#]kCvQ2Mi0&	pQXfB9t81goe&3#L	15d2d420	treongw1-ab9108de 36728
Zenphyr 1.9

##########

Would there be any other settings other than subscribe to related to this 
Two settings:
- saman tien
   + waiting for review
   + 
- koontisähköposti tilaa/ei, once/date - once/week
   + assigned, started
   + assigned, waiting for review
   + assigned, monitoring, started
   + assigned, marked as finished

- assignment manager
   + näkee onko mittaus myöhässä

Millon kävit viimeksi:
   + slack-viiva ECG listassa



#### Operations

https://pulseon.atlassian.net/wiki/spaces/POWS/pages/3041329155/Shared+Scratchpad#Organization-admin-assigns-clinical-role-to-themselves

Update Jari, Jaakko https://pulseon.atlassian.net/browse/GW-87


## Factory

Add a test case that the device is empy when coming from the factory.


## GW characteristic writing method
- uses notifications
- WD 159 ble max packet size
   + effective size is 244

CONFIG_BT_BUF_ACL_RX_SIZE=251
CONFIG_BT_L2CAP_TX_MTU=247
CONFIG_BT_BUF_ACL_TX_SIZE=251
CONFIG_BT_CTLR_DATA_LENGTH_MAX=251


## TODO

Lisää design change registeriin sarake design review, joka täytetään systeemille.

##
Attach a note to a measurement session when sending for interpretation.
A special role for person to receive the summary email. "Doctors don't want that everyone sees the work queue"
A feature to turn off all the emails notifications.



Update Atostek
https://pulseonfi.sharepoint.com/sites/medical/Projects/Forms/AllItems.aspx?id=%2Fsites%2Fmedical%2FProjects%2FAino%20ECG%2FDesign%20Deliverables%2FSoftware%2FConnectivity&viewid=dc6060b4%2D8f6f%2D4c96%2D959a%2Dab25e6ce27b6


## Myyntiversio

Suostuu aloittamaan session akulla, joka on tyhjempi kuin 98%.



## AWS puhelu
using ECS with fargate

suggestions:
- dynamo db as a quick index for data stored elsewhere
- aurora db is completely cloud based
- redis to cache


Cortes Sack, Monica
Security Automations for AWS WAF | AWS Solutions
aws.amazon.com
https://aws.amazon.com/solutions/implementations/security-automations-for-aws-waf/

Managed DDoS protection – AWS Shield Features  –  Amazon Web Services
aws.amazon.com
Defend against most common, frequently occurring network, transport, and application layer DDoS attacks that target your website or applications.
https://aws.amazon.com/shield/features/

Amazon Aurora MySQL PostgreSQL Features | Relational Database | AWS
aws.amazon.com
Amazon Aurora is a relational database service that combines the speed and availability of high-end commercial databases with the simplicity and cost-effectiveness of open-source databases. Aurora is fully compatible with MySQL and PostgreSQL, allowing existing applications and tools to run without requiring modification.
https://aws.amazon.com/rds/aurora/features/

Theoretical cost optimization by Amazon ECS launch type: Fargate vs EC2 | Containers
aws.amazon.com
https://aws.amazon.com/blogs/containers/theoretical-cost-optimization-by-amazon-ecs-launch-type-fargate-vs-ec2/



# Ahjo

Kysy Jarilta mitä tutkimusta tarvitaan ahjon boardille.
https://pulseon.atlassian.net/browse/OHRSW-2159
https://pulseon.atlassian.net/browse/BUGS-56


https://ims.prod.pulseon-ecg.com/Devices/DeviceHistory?deviceUid=(01)06430054330121(10)0222(11)220118(21)000207
Kreikka irrecoverable error: (01)06430054330121(10)0222(11)220118(21)000207

sudo journalctl -u pulseon-app


###

Introduce waiting for release state in PULTEK project
Not stock --> Retired

Add session lenght in week to IMS device history view "Why in weeks"

requestedInstance
Instance address for DMS where device is now allocated.
what if empy?

# IBI data analysis

Added role Doctor, PulseOn Demo System, Sydänsairaala kliininen tutkimus to user https://prod.pulseon-ecg.com/Identity/Account/Manage?userId=88e87111-b9a7-4cbb-bba7-e7d017a43ef6
https://www.dropbox.com/work/Clinical%20Trial%20Limited%20Share/Screening%20study%20documents

estimated end 11.01.2023

######

Atostek
- Is there delay of processing. Seems 10-15 minutes after files are uploaded for ECG. For IBI ~8 hours but should be 10000 IBIs, i.e. 10000/(60*60) ~ 2.8 hours
- Sanitize annotation message PULTEK-767. Could this happen elsewhere?

# External annotation
- marked as finished --> no longer possible to annotate
- marked as finished --> no extra steps to do
- no way to separate by who has annotated  internal vs. interna external

- Whey location ID has a running number instead of GUID
- Do you have a test case for all new issues? What is the criteria to have it as a test or not?
- Supported Windows versions need to be updated

- Release Verification documentation 

- Marko: Go through AINO-DIRs and IMSRs to link the traceability related ones and fill into OPs excel
- Adrian & Marko: Go through new tests since 1.0 to link all requirements


GW installation: start pulseon-reinstall only after iotgw or gw-system-manager has started

# IMS API
requestedInstance has something but it's not valid
lastDMSInstance has something but it's not valid

# What is logged about annotations
creation, changing, event when ready, annotation events

# ECG analyysit
pituus 20-30 sec
onko ECG-mittauksen aikaiset IBIt merkitty huonolaatuiseksi liikkeen takia. pieni haaste aikasynkan takia

10 sec alusta loppuun: yli 50% liikkeen takia

# Findings
- Separate API keys for test/prod IMS

Hidden assumption
- all data is provided in one go
- session started is attached
- session closed event is attached

# Vibra jäi pärisemään

39: 2022-12-19 15:14:24	2023-01-02 10:33:17	13.80	N/A	(01)06430054330121(10)0222(11)220124(21)000365	ΜΑΧΤΟΠΟΥΛΟΥ ΑΙΚΑΤΕΡΙΝΗ	ΠΑΠΑΦΗ 144 ΘΕΣΣΑΛΟΝΙΚΗ 	PROBLEM WITH CONTINUES VIBRATION/RETURNED BACK


# Windows 11 apps to install

- putty, droidcam, brave, SteelSeries GG, Discord, Git, Subtitle Edit

- 30 pcs (some to Jari, some the Kyrel)

# Questions for Adrian:
- https://pulseon.atlassian.net/browse/AIVER-16 is tested by AIVER-2
- https://pulseon.atlassian.net/browse/AIVER-24 added Component Service
- https://pulseon.atlassian.net/browse/AIVER-27 added Component Service
- https://pulseon.atlassian.net/browse/AIVER-30 Should we add chgin error - KUISMA 
- https://pulseon.atlassian.net/browse/AIVER-31 link same as https://pulseon.atlassian.net/browse/AIVER-29
- https://pulseon.atlassian.net/browse/AIVER-33 add "Relates to" to dirs mentioned in the Aino Design Verification Plan
- https://pulseon.atlassian.net/browse/AIVER-48 Should we link Atostek requirements and testing?
- https://pulseon.atlassian.net/browse/AIVER-49 added tested by https://pulseon.atlassian.net/browse/AIVER-143
- https://pulseon.atlassian.net/browse/AIVER-50 verification method is Atostek verification
- https://pulseon.atlassian.net/browse/AIVER-51 verification method is Atostek verification
- https://pulseon.atlassian.net/browse/AIVER-51 we should get data for this now
- https://pulseon.atlassian.net/browse/AIVER-52 link to actual requirements
- https://pulseon.atlassian.net/browse/AIVER-54 is this automated, how about https://pulseon.atlassian.net/browse/AIVER-149
- https://pulseon.atlassian.net/browse/AIVER-56 Should we link the SGS report?
- https://pulseon.atlassian.net/browse/AIVER-57 Should we link the SGS report?
- https://pulseon.atlassian.net/browse/AIVER-58 hw-test-plan label
- https://pulseon.atlassian.net/browse/AIVER-59 usability-test-plan, hw-test-plan?
- https://pulseon.atlassian.net/browse/AIVER-60 usability-test-plan
- https://pulseon.atlassian.net/browse/AIVER-66 we could add aiver-143
- https://pulseon.atlassian.net/browse/AIVER-67 we could add aiver-143
- https://pulseon.atlassian.net/browse/AIVER-68 Investigation ongoing about sydänsairaala study
- https://pulseon.atlassian.net/browse/AIVER-67 usability-testing
- https://pulseon.atlassian.net/browse/AIVER-68 sgs-testing
- https://pulseon.atlassian.net/browse/AIVER-69 usability
- https://pulseon.atlassian.net/browse/AIVER-72 Should we add a test about exported sessions or link atostek test?



Is this WD software?
- https://pulseon.atlassian.net/browse/AIVER-43
- https://pulseon.atlassian.net/browse/AIVER-44
- https://pulseon.atlassian.net/browse/AIVER-46
- https://pulseon.atlassian.net/browse/AIVER-47
- https://pulseon.atlassian.net/browse/AIVER-48

Tests
- https://pulseon.atlassian.net/browse/AIVER-145 never run
- https://pulseon.atlassian.net/browse/AIVER-149 could be linked to USB and BLE requirements
 
 
