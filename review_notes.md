## Data integrity procedure

At PulseOn, the identification & traceability information may be linked to data in one of the following methods:
last bullet covers test management tool?

product development data
software functionality
CI system test reports
software trace logs


Typos that could be fixed for the next version: "piece f information", "the data the form of automatically of manually created records"

monitoring of post-market device safety & effectiveness
cyber security aspect


## Product development procedure

Typos to fix in the next version: "If often is advantageous". "mandate a   to organize"

Section 12.3 says "The correct verification method shall be documented in the task assignment". However, the SW development plan defines a common verification method (code review and testing) for tasks so each task does not need to have that in the description. Is this fine?

## WD usability evaluation plan

Some typos that could be fixed in the next version: missing period in "testing process for the Aino wrist device", unnecessary capitalization in "who Is supervising".

Possible questions to add in Appendix Formative A: Are there accidental ECG measurements? Is the ECG measurement accidentally stopped too soon?

## Outsourcing URS Linicone Straps

Changes to fix in the next version: Typos "patien", "potentia". First row is duplicated in the table in section 4. Competence Requirements.

Please use spell check in the next version. Found typos: aquisition, Manufacturinfg, neglible, patien, ther potentia, througout, complaince, the the, Cleaness

## WD UI document

Some improvements for the next version. Describe UI with USB (PC) and BLE (gateway) connection. Describe the predictive battery low alert functionality (https://pulseon.atlassian.net/browse/OHRSW-1207) in the subloop VI. UI description uses t_sense and t_start as measured times but they appear as thresholds in Visio drawing.

## Document and record control procedure

Typos to fix in the next version: "shall be document", "theu", "is die to", "dstrobution", "trainingto", "notpractical"
Inconsistent fonts in section 2.1 Acronyms and Table 2.


## Outsourcing procedure

Typos to fix in the next version: desing, Specificaton, determied, detailled, signatureof 

## Assembly design transfer reports


Section 4: "Regulatory requirements compliance shall be verified during the Design Transfer" doesn't fit in the report. They should have been verified.
Section 8.2.1 "The data stored in the data base shall be download for long term storing to the PulseOn cloud service (SharePoint) automatically". work automatically should be removed.
Section 8.5. Should be changed to correspond with what section 11 states.


PODMS-1378432600-5699	Aino ECG SW Algorithms Test Plan
PODMS-1378432600-6131	AinoECG SW Test Plans Xray Report


Should Section 3. also list the MDR Annex VI part C 6.5.2. requirements for new UDI-DI?
I would use same serial number format for system as for WD, i.e. 8 characters.

## Purchase Procedure

Table of Contents has old heading "Storage TÄHÄN"
Typo to fix in the next version: "ans"

## Atostek AINO-ylläpito
T2109-4495-1 - Atostek - PulseOn - Aino-ohjelmiston ylläpitosopimus.pdf:
Käytetään SOUP ja SOAP sekaisin, mutta tarkoittanee samaa.

## Risk Management Report

Kappaleeseen 8.7. Cybersecurity-Related Risks voisi lisätä maininnan MDGC 2019-16 noudattamisesta

## IBI synchronization
The performance requirement(s) should be more specific e.g. use the limits that are given as acceptance criteria for the item qualification testing. Add a requirement for the input data formats. I believe creating some accompanying documentation was also a requirement defined by Antti. We should probably add that as well.

## Aino ECG Hardware Verification Plan and Report
- Changes to the Previously Approved Version should only list changes from 1.0 to 2.0
- List PODMS-1378432600-6195 Watertightness and Chemical Resistance of Aino ECG WD.docx as an associated document. PODMS-1378432600-6195 should be approved.
- List PODMS-1378433600-7044 Aino ECG Surface Temperature Test Report.docx as an associated document.
- Aino ECG Hardware Verification Plan and Report (this document) seems to duplicate the test cases in PODMS-1378432600-6195 Watertightness and Chemical Resistance of Aino ECG WD.docx. Make sure that they are identical in both or remove them from PODMS-1378432600-6195 and refer to Aino ECG Hardware Verification Plan and Report (this document) instead.

AINO-DIR-006 Chemical Endurance material study:
- Is the IPA immersion actually done as part of AINO-DIR-006 Chemical Endurance Exposure Tests? If so it should be removed from this table.

The field "device/software/document identifier and version" is used wrong or doesn not include the versions in many cases:
- AINO-DIR-006 Chemical Endurance material study
- AINO-DIR-007 Material irritation effects test
- AINO-DIR-017 The wrist device shall not have a display
- AINO-DIR-010 The wrist device shall have a separate charger and a charging dock
- AINO-DIR-067 The wrist device shall meet all the applicable requirements of the WEEE electrical waste directive
- AINO-DIR-068 The materials used shall meet ROHS requirement

## PODMS-1378432600-6134 Aino ECG WD Home Health Care Test Plan.docx
Broken image link in section 5.16

## Aino ECG Factory Tests Requirement Specification
Kappale 2: puhuu "Aino verification". Varmaa kopiopasta.
Voisi lisätä myös viittauksetn PODMS-1378432600-5774 AinoECG WD SW Connectivity, josta protokolla löytyy

## Read Report Powershell Script

### Type Qualification
Some quick comments:
- Add Adrian Constantin as a reviewer. OP might not be that relevant reviewer.
- Section 2: Specify the used git commit as the version. Something like repository https://github.com/PulseOn/manufacturing-reporting-tools commit 0ebab7d4197351ebc8cf6749954dbc04eb2de0b4).
- Section 3: There should be some evidence of the IQ, e.g. the output of running the script itself. Also, the environment should be documented, e.g. OS build, PowerShell version, Microsoft.SharePointOnline.CSOM version.
- Section 6: Is this automated manufacturing tool? If yes, it should be requalified 1/year according to PODMS-942620546-1457 Equipment & Software Tool Qualification Procedure. If not, should it be requalified if Windows OS, PowerShell or Microsoft.SharePointOnline.CSOM is updated?

### Item Qualification
Some quick comments:
- Add Adrian Constantin as a reviewer. OP might not be that relevant reviewer.
- Specify the used git commit as the version. Something like repository https://github.com/PulseOn/manufacturing-reporting-tools commit 0ebab7d4197351ebc8cf6749954dbc04eb2de0b4)
- Section 3: There should be some evidence of the IQ, e.g. the output of running "Get-Package Microsoft.SharePointOnline.CSOM" and then running the script itself. The Microsoft.SharePointOnline.CSOM version is also relevant to document.
- Section 6: Should the script be requalified also if the Microsoft.SharePointOnline.CSOM is updated?


### Aino ECG WD and System Complementary Verification Plan - EN 60601-2-47

Kappale 1.1 Lisäsin Aino ECG WD and System Complementary Verification Plan - EN 60601-2-47 ja muutin kieliasua.
Kappale 3 Lisäsin Aino ECG WD and System Complementary Verification Plan - EN 60601-2-47 ja poistin SharePoint sijainnit, koska ne saattavat muuttua.
Kappale 4.3.1 lisäsin puuttuvan kuvatekstin kuvalle 2
Kappaleessa 4.3.2 näyttäisi jääneen lause kesken: "Thue it is adequate to test the device with one" En osannut korjata tätä.
Kappale 4.3.4 Intended use oli vanha versio. Päivitin uuteen.
Kappale 4.4.1 Onko näin? En ainakaan huomannut versionumeroita draft raportissa.
Kappale 4.4.1 Onko tätäkään tehty?
Kappale 5 Tein muutamia kieliasumuutoksia

### Aino Clinical Evaluation Plan
Section 7.9: Typo "wrist deice"
Section 7.9.1: PPG is said to use "green color light". Typos "interals", "Wrisband", "finnish"
Section 9.3 Weird line break

### Aino ECG Master Design Transfer Plan
OK with the changes but more information about the actual details (eg. what "has been agreed") need to be added in the next version to all sections. Also the "shall" points need to be converted to what was actually done. Links to the documents where those are detailed is also enough.

## Demo product

- Lisää dokumentin nimeen AMS-1 ja voisi myös laittaa kaikki alkukirjaimet isolla, kuten on tapana
- Täytä etusivun tyhjät kentät ja roolit (koska lukee name & role)
- Kappale 2: Pitääkö mainita jotain datan omistuksesta?
- Kappale 3 (vai joku muu): Voisi lisätä selvennyksen, että jokainen paketti sisältää oman käyttäjän ja oman organisaation
- Kappale 4: Lisää Windows version (10?) ja selain, joka asetetaan oletukseksi (Edge?)

## Capa Procedure

Typoja: "indictes", "complince", "shal", "ba", "Competene", 
Kappale 6.3. taulukko 4 ensimmäinen rivi. Pitäisikö lisätä Software Development Procedure?

## AMS-1 Operations Manual

Lisää seuraavaan versioon:
- käyttäjien poistaminen/muuttaminen
- asiakkuuden lopettaminen


6.3.3 The ISO and and BSI standards/certifications should be added to the references and referred in the text
8 "High availability can be achieved" --> If I were a customer I'd wonder if "Is it achieved?"
9 The IEC guidance document should be added to the references (§3) and referred in the text. Same for AES standard

### 0.16



## Aino ECG Factory tester Qualification Plan and Report

Pidetäänkö tätä koko tuotantotestauksen kelpoistuksen ylätason dokumenttina vai pitäisikö laatia ihan oma yhteenvetodokumentti? Haluaisin, että jossain selvennetään mitä kaikkia vaatimuksia tuotantotestaukselle on (ilmeisesti ainakin PODMS-1378432600-5350, PODMS-477950017-5515, PODMS-477950017-5606?), mitkä testerit toteuttavat mitkäkin vaatimukset ja miten  eri vaatimusten/testereiden kelpoistus on jaettu eri dokumentteihin.
Esimerkiksi vaikuttaa, että Aino ECG Factory Tester Modules Requirement Specification määrittelee vaatimuksia, joista AinoTester2 täyttää osan. AinoTester2 täyttävien vaatimusten kelpoistus on ilmeisesti jaettu Aino ECG Factory Tester GW part Qualification plan and report ja Aino ECG Factory Tester Modules Qualification plan and report dokumentteihin. Osittain vaikuttaa, että vaatimuksen ja testin linkitys on ID:n avulla, vaatimuksen ID on myös testin ID. Tämä on vähän hämäävää itse testille voisi keksiä on 
Joku taulukko näistä linkityksistä antaisi edes jonkinlaisen mahdollisuuden todeta, että kaikki vaatimukset on täytetty 

Onko kaikki vaatimusdokumentit päivitetty ajantasalle? Entäs Aino ECG Factory Tester Version Information?

1. Tässä pitäisi selventää mihin vaatimuksiin ja testeriin tämä kelpoistus liittyy.
2. Tähän pitäisi listata vaatimusdokumentit, jonka perusteella testataan. Onko tässä tapauksessa pelkästään Aino ECG Factory Tests Requirement Specification?
4. Tähän pitäisi listata mitä testereitä kelpoistus koskee ja kerrata mitä vaatimuksia vastaan tässä testataan.
6. Testeissä pitäisi kertoa millä testerillä se on suoritettu, jos useita. Kaikille testeille ei löydy vaatimusta, esim G0.1.
8. Kannattaako tätä hyväksyä edes tässä vaiheessa, jos joku testi pitää kuitenkin toistaa?


## Design change label material

Musta Jarin kuuluisi olla katselmoija.
Pitäisikö kappaleessa 2.4 ehdotukseen sisällyttää myös toimittajan vaihdos?
Kappaleessa 3.2 mulla ainakin herää kysymys, että eikö voi mitenkään vaikuttaa bioyhteensopivuusriskiin?

Sitten samassa kohdassa tai vasta B-osassa todetaan vaikka että myös uuden toimittajan materiaalit löytyy UL:n listalta linkkeineen. -> samaa materiaalia eri tuotenimi -> ei muutoksia bioyhteensopivuusriskiin.


## Aino ECG Instructions for Batch release

Poista kommentit dokumentista.
Kappaleessa 9. suluissa oleva dokumentin nimi ei ole niin selkeä tapa. Muutaisin samaan tyyliin kuin kappaleessa 10. eli Report file is xxxxx.
Muuta kappaleiden 10 ja 11 nimet samaan tyyliin kuin kappale 9.

## Aino ECG Production Description B3

Sections 5 and 6: Should the version number of each document be specified so we know the whole process for B3? This is also related to the FDA discussion.

Section 9.2 sentence "When the production has been successfully transferred to the manufacturer" is weird in this context. The design transfer has occurred a long time ago so I doesn't need to be mentioned here with batch 3.

Section 12.1 It was quite hard for me to understand the point about not marked serial numbers in the database. Maybe reformulate this to something like: Due to a human error the serial numbers of some boards that were reworked during the AOI phase were not recorded in the rework database.


## Aino ECG Production Description B4 onwards v1.8

Kommentit
- 9.2 Tuo kohta "When the production has been successfully transferred to the manufacturer" on vähän hassu, koska tässä jo tehdään batchia 4 ja eteenpäin jolloin tietenkin design transfer on jo tehty.
- 9.3, 9.4, 9.5: Kannattaako sales boxien sisältöjä laittaa tähän vai vaan viitata dokkareihin, josta se löytyy? Mulle sopii näinkin, mutta jos muuttuu tai tulee uusia, niin pitää sitten tämäkin muistaa päivittää.
- 9.3: Batch release kohdassa voisi viitata PODMS-1378432600-7802 Aino ECG Instructions for Batch release -dokumenttiin.
- 11.1: Lisää viittaus akkujen vuosihuoltoon ja tarkenna mitä much longer than one year tarkoittaa (tarkennus voi olla tuossa vuosihuolto-oppaassa).
- 12.1: Onko B4> laitteissa edelleen tehty tuota "Unfortunate human error"?
- 12.2 ja 12.3: Kuulostaa, että nuo "separate guidance" ja "Separate emails" pitäisi olla tallennettu SharePointiin


## Aino ECG Production Description B4 onwards v1.11
- Kappale 5: Virheellinen dokumentti-ID POMDS-1378432600-7802
- Kappale 9.2: typo "changeling". En oikein ymmärrä mitä viimeinen lause "At the end of the production the production batch released before it was stored into the warehouse or delivered to the customer" sanoo.
- Kappale 12.1: Eikö tämä ole kuvaus miten tehdään myös jatkossa batchien osalta? Tuo "were marked" muoto on siinä mielessä väärä.


## Aino ECG Instructions for Batch release v1.3.

- Dokumentin nimessä voisi käyttää isoja kirjaimia johdonmukaisesti eli nimen muuttaa "Aino ECG Instructions for Batch Release"
- Lisää kappaleeseen 12.3 selvennystä, että kyseessä on Jira taski AMS-1 Operations projektissa
- Lisää sopivaan kohtaan linkki käytettyyn Jira projektiin https://pulseon.atlassian.net/browse/AMS1OPS

## AMS-1 Software Security

Minusta kuvauksesta ei käy ilmi, mitä tietoja potilaasta ja ammattilaisesta tallennetaan järjestelmään. Tässä etenkin henkilötiedot tai tiedot, joilla voidaan tunnistaa henkilö.
- Lisätty kappale 6

Web-käyttöliittymä on ilmeisesti ainoastaan ammattilaisen käytössä. Miten ammattilainen saa käyttöoikeudet, mitä tietoja ammattilaisesta kirjataan tunnukseen ja miten käyttäjätunnistaminen toteutetaan. Käyttöoikeustasot taisi olla.
- Tietoja lisätty kappaleeseen 7. 

Mainitaan, että järjestelmän tietokanta on salattu, mutta salausavaimen hallinnasta ei ole kuvausta.
- Muutama selvennys lisätty kappaleeseen 8.

## Document and Record Control Procedure

3.1: Mites tuotantodokumentit? Ne ei ole Aino Document Registerissä.
4.4: Pitäisikö tähänkin lisätä maininta sähköpostista tai muusta kuten 6.2. Mitä tarkoittaa Direct Recipients ja CC kenttä?
4.9.	Document Retention: Should we add patinet data and logs?
4.6.2 Table 6: Onko tämä mahdollista kaikille dokumenteille? "adding an “Impact Analysis” sheet in the beginning of the document"
6.1.1: Olen käyttänyt approve flowta ilman docusignia. Onko OK?



## Aino ECG battery aging in shelf-mode verification plan and report
- Pitäisikö Antti laittaa myös katselmoijaksi, kun tiettä myös paljon näistä asioista?
- Laita alkuun tarkka syy sille miksi dokumentti tehtiin. Jotain tyyliin, että se on verifioimaan vaatimusta, että rannelaitteen shelf-life on 3 vuotta, joka on määritetty user guidessa (vai missä toi nyt on?).
- 6.1:
  * Kuville pitää olla selkeä lähde mistä otettu.
  * Selitys mistä DTP140757 tulee (ilmeisesti ranneltaitteen akkumalli. viittaus HW design dokkariin)
- 6.2:
  * Alkuun selitystä mikä shelf-mode on ja mistä akun kulutus siinä tilassa koostuu: laite menee shelf-modeen, kun se ei ole mittaustilassa. Laite on oheistettu varastoimaan niin, että akku on ladattu täyteen. Käytössä laite menee shelf-modeen, kun akku on 8%, mutta laitetta ei pidä varastoida näin.
  * Shelf-modessa mcu ym. on pois päältä ja vain RTC, safety circuit, power switch circuit ym. pakolliset on päällä. Tässä olisi myös hienoa viitata HW design dokkariin. Viittaus dokkariin, jossa 1 uA virrankulutus on mitattu olisi hieno.
- 6.3: energy mount --> amount of energy
- 6.4:
  * "as we can see from previous" tässä jäänyt pois sana, mikä previous? Ehkä Section 6.1?
  * En ymmärrä miten tämä "the voltage and charge drops much faster at very first moments of the storage" ja pari seuraavaa lausetta perustelee lineaarisen interpolaation pessimistisyyttä. Eikös pessimistisyys tule siitä, että loppuosassa tyhjenemisnopeus hidastuu? Ei se, että alussa tyhjeneminen on nopeaa.
  * taulukko "Voltage after 3 years (V)" --> "Calculated voltage after 3 years (V)"
  * "This is just a concern long term storage of the battery. During normal use the low voltage condition is not an issue at all" Jotain perustelua näille, ilmeisesti että laite katkaisee virran hyvissä ajoin ennen kuin 3,6 saavutetaan ja että lyhytaikainen varastointi tuossa jännitteessä ei aiheuta ongelmia akulle (tähänkin olisi kiva joku lähdeviittaus).
  
 ## SW Development Procedure
 5.2 "SE requirement"
 8. the deliverables of each sprint shall be verified/validated in a documented manner and approved formally
 10.1 SW Maintenance Plan
 
 8.1.	System Testing
how integration is done?

## Document Management System - Architecture
Figure 1. should be updated. I'm not sure wha the SharePoint --> GitHub document links mean. Also, Jenkins WD release artifacts are exported to SharePoint (what about others?). Xray reports are exported to SharePoint.
Section 5. Maintenance: E.g. SharePoint, Jira, GitHub are updated automatically by the manufacturers. Should something be said about that?
Manufacturing
Atostek QMS


## DTAC_PulseOn

B4: Markku, Tuomas
A user journey (or customer journey) is a scenario-based sequence of the steps that a user takes in order to accomplish a high-level goal with a company or product, usually across channels and over time.

## Design Change Form Template
Design change:
1.3
miksi lisäys: approved product version**:
5.2: Major change aika herkästi
change intends to significantly affect device safety or effectiveness (e.g. significant improvement of clinical outcome, mitigation of a known risk, response to an adverse event, etc.)
change which introduces new hazard(s)/hazardous situation(s) which is/are not acceptable without mitigation actions (see §3.7)
any design change which verification/validation results indicate any unexpected issues (please see §8.3.)



## SharePoint OQ/PR 2023

OK, vaikka tuo kappaleen 4.1 kommentti "operation/performance observed with [...] document library, etc. can be safely generalized to all the other corresponding system elements." EI selkeästi päde, koska kirjastoilla on erilaisia konfiguraatioita (esim versionumero rikki, jos dokumentin siirtää Project -> Products). Olisi hyvä, jos konfiguraatioiden oikeellisuus tarkistettaisiin myös jatkossa osana kelpoistusta. Onko konfiguraatioita dokumentoitu johonkin?

## Jenkins Installation and Configuration 0.10

1.1: typo: "used for the development software". Could mention algorithms in DMS (Beat and ECG quality).
1.2: typo: "the VCS move the software"
5.3: Is "PulseOn Android Application repository" needed?
5.4: typo: "apt get"
7.9.1: typo: "authorized kyes"

## User Guide Jan 29, 2024 15:45


General:
  - Sections could be links for easier access.
  - See image titled. Could be link and number.
  - 5.6.2.2. has links to figures by number
  - "should be"

1.3.2: "The automated analysis software (ECG Parser) is not complete diagnostic ECG software. Only beat and rhythm classification, HR and HRV interval measurements are validated in the ECG Parser output. Other output parameters may be used for indication only."
1.3.2: typo: "A wet environment, such as a shower, can cause accidental ECG measurements to start and the device may then the relevant notifications erroneously"
1.3.2.: typo: The device and its accessories must not be serviced or undergo maintenance on while being worn or in use.
1.3.3: different font: The wrist device is not intended to be used on people who have a pacemaker.
1.3.7: wording: However, the wrist it is worn on can be alternated.
2.1:   wording: for possible monitoring by the doctor.
2.1:   is this neede: The DMS may also be locally deployed on the hospital premises to be hosted on the hospital IT infrastructure.
2.1.1:
  - more like 5 months (50 ECGs per day, 1 month if 90 ECGs per day)
  - Should we drop? Apple Safari
  - Workstation requirements
2.2:
  - Device components described in multiple section:
  - wording: wrist-wearable, wrist-worn device, wrist device
2.2.1.1: link to Recharging section
2.2.3 The computer needs to have the Data Transfer Software installed. "and running"
3.3: typo: take a ECG measurement
3.4.3
  - Notifications could come before taking ECG.
  - Logic is very hard to follow.
  - Table 3 could have action column on what to do: e.g. take and ECG
3.4.5: typo: docked
3.6:
  -  Optional using gateway: Should charging dock be optional?
  -  "but not part of it" is confusing to users
3.6.1:
  -  Model number: 1111. Should add 1211
  -  LTE NB-IOT	has been disabled (instructed by Treon not to use)
3.6.2: do not use the PulseOn device. Should this be about gateway?
4.1.: The wrist device needs to be linked to the patient in the Data Management Service.
5: a local installation of DTS: what is local?
5.2:
  - typo: The ECGs measurements
  - the software this document refers to. This section
5.3: Doctor and nurse have same functions
5.4.1: URL of the DMS deployment. What is this?
5.4.6: delete user data?
5.5.1: A Customer System, or DMSSystem. What is DMSSystem? Should we include SuperUser functionalities?
5.5.2: Figure 25. Organization system listing is a bit weird.
5.5.2.1: An administrator is required to set the two-factor authentication to forced if the installation is publicly available.
5.5.1.2:
  - See image titled. Could be link and number.
  - NOT TRUE: At least one ContactPerson is required for each Customer/DMSSystem.
5.5.2.3:
  - External organization not explained
  - Figure 29 quite small
5.5.2.4: It should be kept in the system for traceability. --> it is
5.5.3	User Management could be before system and org stuff in manual
5.5.3.1.:
  - role selection quite detailed walkthrough
  - typo: NOTE: The user organizations added can belong only to Internal or External Organizations
5.5.3.2:
  - Different font: Creating a User
  - Disable 2FA could be own section.
  - NOTE: MFA mentioned once, 2FA 40 times
6.5.1.2:
  - late or that the measurement session is late for review. Should it be explained more what it means?
  - FILTER --> SEARCH
  - Figure 38. Red boxes: The red parts of the image are not part of the software and were added for clarity.
  - MODIFY --> EDIT
  - Not available: ARCHIVE PATIENT
  - Figure 39: Should be change Cancel RED?
  - EDIT PATIET --> SAVE CHANGES
5.6.2:
  - Could link to section on Using the device.
  - the device
5.6.2.1: Figure 41: colors incorrect
  - Not necessary: with an authorized user logged in to the DMS
5.6.2.2.: Figure fort weird
  - Is the difference clear?: DTS applications context menu
5.6.2.3:
  - (i) is weird
  - Data transfer info in weird place. Could be somewhere in upload section.
5.6.2.3.2	Measurement Session Week View
  - I would put the image to viewing data section
  - not correct: the wrist devices IBI sensor
  - difficult sentence: The circled numbers indicate ECG measurements of the selected week, which will be displayed as circles, at their appropriate day of the week and time of day
  - what? Annotated ECGs will also be distinguishable
5.6.2.3.3:
  - NOT TRUE: Each segment will be coloured according to the same logic as the days in the week view
5.6.2.3.4:
  - Not exactly true: The measurement session day view will contain all the ECG measurements taken during that day
  - typo: algorhithm
  - Could be reworded more nicely: Directly from device
5.6.2.3.5.:
  - red dot at end.
  - Maybe too many: All data should be reviewed by a healthcare professional. 
  - ? to which the User has access.
  - Why should? The zoom reset button should undo this action.
  - Why should and clearly? The interface should clearly display the length of the measured area in milliseconds.
5.6.2.3.7:
  - Not true. Old image: With a single ECG measurement highlighted, the ECG annotation-related functionalities will be available to the User.
  - Not true: Annotations of the measurement session --> Session annotations
5.6.3:
  - weird wording: an easy-to-operate wrist device to take ECG measurements in everyday life
  - what? signal quality level
  - what? “no signal” and “no beats detected”
  - Table 8: do we show all 12?
5.6.4:
  - Update: “Export the measurement session” and “Export annotated ECGs”.
  - The user cannot navigate around during this time



SIVULLA 80

# AMS-1 Periodic Safety Update Report
Comments
- Section 2. has larger font in the start of 2nd paragraph, which looks out-of-place.
- Section 7.3 I would undertand some ongoing process by the expression "until perpetuity" but the calculation has been done and there is an actual end date. I would usggest using the actual end date for when the calculation was made instead.
- Section 7.4 typo "was analyzed algorithm team"
- Sections 7.5 and 8. use "Aino", which could be changed to AMS-1 device.

# Management Review Meeting Agenda & Minutes Template v1.5
- Document Title is "[Date]", which could be changed to something more descriptive.
- Should the Net Promoter Score (NPS) be deleted from 12.1 as well?

# Aino Device Tester Tool Type Qualification Form v0.7
- Point of type qualification is to check that tools is ready to be tested
- Planned to be tested --> a test case has been implemented


# Design Change Procedure v4.6
- Section 2.1: typo "prectices"
- Figure 1: arrowhead missing from significant change -> yes
- Section 4.2: typo "Corrections actions"
- Section 4.2: "allow access to device-related services" could be reworded to "restore access to online service"
- Section 4.3: typo "chage"
- Section 4.4: typo "Design Change For"
- Section 4.5: typo "If change proposal rejected"

# Post-Market Surveillance Procedure v3.20
MDCG 2019-16 ohjeistuksen voisi mainita referensseissä ja sen mukaisesti voisi lisätä tietoturva-asiaa vielä explisiittisemmin useampaan kohtaan, esim.
  - Taulukko 2. "devices shall be safe and secure in their intended uses/purposes"
  - Kappale 5.5. voisi mainita, että security incident voi myös mennä tähän kategoriaan, jos sillä on suoraa tai epäsuoraa vaikutusta turvallisuuteen (MDCG 2019-16 Annex II).
  - Security melkeimpä joka kohtaa, jossa mainitaan safety, esim kappale 6.1.1. "quality, safety, security and performance"
- Kappale 5.3: Käytännössä palautteen vastaanottaja ei välttämättä osaa tehdä arviota tarvitaanko "immediate actions". Tähän voisi laittaa, että mikäli vastaanottaja on epävarma arviosta niin ottaa yhteyttä reponsible area owneriin.
- Kappale 7: Eikö Immediate Actionsit ole nyt mukana Design Change Producuressa eli voisi mainita, että toimitaan sen mukaan.

# Management Review Meeting Agenda & Minutes 12.03.2024.docx v0.8
Poistaisin muutokset Changes to the Previously Approved Version kappaleesta.

# Purchase Procedure v7.6
- Aino voisi korvata AMS-1

# RMT Meeting Minutes 2024-05-16
Front page:
  - version is incorrect in "Aino 01.00.12 System Release". This could be changed to "AMS-1 01.00.13 System Release"
  - Row "10" should be "Time" I suppose.
Section 4.
  - Only DMS/IMS/DTS bugs are in "Atostek's Jira". Others are maintend by PulseOn.
Section 4.2:
  - Again this was not only Atostek’s risk assessment but combining the assesment of both Atostek and PulseOn Jira projects.

# Aino Risk Management Register 3.28
CHANGE HISTORY: näyttää olevan aika vanha.
Muita huomioita: DEVICE OVERVIEW: Pitäisikö  olla "PulseOn Arrhythmia Monitor System" ja pitäisikö version olla ensimmäinen CE hyväksytty systeemiversio 01.00.01?

# SharePoint Online Tool Item Qualification 2024 v0.7
Metadata: Reviewers are wrong.
- Header: Document version wrong.
- 3.1: "responsible person" and "IQ need assessment" empty
- 4.1: "SW installation-specific assessment", "need for PQ" and "manufacturer’s OQ forms available" empty
All test cases: I would like to see the library (and other relevant information if any) where the test was done in the test notes because we have - different configurations in different libraries.
- 4.2	OQ/PQ Breakdown: Reference to URS should use the requirements defined in the Type qualification form
- OQ/PQ - 04: "The file can be accessed from both searches directly." does not seem to be tested.
- OQ/PQ - 09: "Repeat step one and two from OQ/PQ – 08..." Should this be steps 2. and 3.?

# SharePoint Online Tool Type Qualification 2024 v0.2
- Metadata: "Changes to Previously Approved Version" seems to apply to the template and no the document in question.
- Header: Document version wrong.
- Section 4: Does SharePoint really not require any configuration? Wouldn't it be used for data manipulation, transfer and visualization?
- Section 5: If OP is responsible for DQ, he should be reviewer.
- Section 5.1: This is a requalification so "in case of requalification" should be filled for each URS.

# SharePoint Online Tool Type Qualification 2024 v0.2
- responsible person for URS role missing

# SharePoint Online Tool Item Qualification 2024 v0.8
3.1 item configuration** on valittu no, mutta silti alempi kohta, jossa lukee "if yes,.." on täytetty
4.1: edelleen paljon kohtia tyhjänä
OQ/PQ - 04: "The file can be accessed from both searches directly." vaatimusta ei ole huomioitu testauksessa tai ainakaan siitä ei ole mainintaa
Onko URS-ID 1.7.5 jätetty tarkoituksella testaamatta? Mulle sopii olla testaamattakin, mutta pitikö johonkin perustella miksi ei testata?

# Quality Manual v 7.8
- Changes section?
- 7.5.6: Should there be a mention about cloud service deployment?
  "Software deployment doesn’t contain any stages which require validation because the release packages’ correctness may be verified before their deployment to the manufacturing partner. However, automated processes utilized during compilation of the release packages shall be validated appropriately"
- 7.5.8: UDI is not used in manufacturing at all steps?
- 7.5.10: Is data pseudonymized?
- Chapter 7.5.10: clarified protection of patient data.
- Chapter 7.5.11: added description of how medical device software is protected from unauthorized 

# Design change UDI
- Section 1.3: Approved AMS-1 version in Singapore is 01.00.06
- Section 2.7: Add Singapore as target market. The device is not yet approved in Saudi-Arabia so that should not be a target market.

# Software Development Procedure 1.6
- Typo: "nay contribute"
- Section 10. Software Maintenance intro could include keeping SW state of the art as an intention since its required by the MDR.
TODO:
  - SW risk control methods as SW requirements
  - patches and obsolescence of SOUP.

- Include Jaakko in the review flow or remove him from the document front page.
- Replace SFS-EN 62304 --> IEC 62304
- Add maintaining state of the art as an intention in section 10.

# RMT meeting minutes
- Header page:
    + System version is incorrect in header page
    + System Design Change version number is incorrect as of now but this could be on purpose.
- Section 3. Wrist device hardware version 1.4 could be added in the heading
- Section 4. Correct DMS version is 01.09.00
- Section 4.1.1.2.: It could be added that the file is automatically quarantined if scanning finds malware.

# CAPA-037 Form v0.1
Document "PODMS-1416550729-5734 AMS-1 - List of Applicable Standards" does not exits. It should probably be "PODMS-1378432600-5734 AMS-1 - List of Standards"

# AMS-1 Risk Management Plan v4.3
- Section 2: Add cybersecurity risk document