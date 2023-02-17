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
ssh -C -i ~/.ssh/gw_key -p 32637 gwadmin@localhost
APWD: Wbw4C(O[WEmgGOKt

]
## Jari
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

Adrian: mental block on setting up the Windows worker.

HUOM laskutusjärjestelmämuutokset!!
mittauksen pituus valittavissa viikon blokeissa, laskutus menee valitun pituuden mukaan

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
office 2 (jarin pöydällä): treongw1-5a58679a
ssh -i ~/.ssh/gw_key gwadmin@treongw1-5a58679a. 'sudo dbus-send --system --print-reply --dest=org.ofono /ubloxmodem_0 org.ofono.NetworkRegistration.GetProperties'
ssh -i ~/.ssh/gw_key -p 32721 gwadmin@localhost

## GW debugging

	vim /lib/systemd/system/ofono.service
vim /lib/systemd/system/bluetooth.service
/usr/lib/ofono/test/list-modems
python /opt/nbiot_connection/ofono_control.py -v -w --scan

dbus-send --system --print-reply --dest=org.ofono /ubloxmodem_0 org.ofono.NetworkRegistration.GetProperties

Download 32.1KB/s

#####
ab9108de	352373197141323	scNGz#]kCvQ2Mi0&	pQXfB9t81goe&3#L	15d2d420	treongw1-ab9108de 36728
Zenphyr 1.9



##########

- Aino Document Register
- Operations manual hyväksyntä
- 


