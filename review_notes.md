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

Table of Contents has old heading "Storage T??H??N"
Typo to fix in the next version: "ans"

## Atostek AINO-yll??pito
T2109-4495-1 - Atostek - PulseOn - Aino-ohjelmiston yll??pitosopimus.pdf:
K??ytet????n SOUP ja SOAP sekaisin, mutta tarkoittanee samaa.

## Risk Management Report

Kappaleeseen 8.7. Cybersecurity-Related Risks voisi lis??t?? maininnan MDGC 2019-16 noudattamisesta

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
Voisi lis??t?? my??s viittauksetn PODMS-1378432600-5774 AinoECG WD SW Connectivity, josta protokolla l??ytyy

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

Kappale 1.1 Lis??sin Aino ECG WD and System Complementary Verification Plan - EN 60601-2-47 ja muutin kieliasua.
Kappale 3 Lis??sin Aino ECG WD and System Complementary Verification Plan - EN 60601-2-47 ja poistin SharePoint sijainnit, koska ne saattavat muuttua.
Kappale 4.3.1 lis??sin puuttuvan kuvatekstin kuvalle 2
Kappaleessa 4.3.2 n??ytt??isi j????neen lause kesken: "Thue it is adequate to test the device with one" En osannut korjata t??t??.
Kappale 4.3.4 Intended use oli vanha versio. P??ivitin uuteen.
Kappale 4.4.1 Onko n??in? En ainakaan huomannut versionumeroita draft raportissa.
Kappale 4.4.1 Onko t??t??k????n tehty?
Kappale 5 Tein muutamia kieliasumuutoksia

### Aino Clinical Evaluation Plan
Section 7.9: Typo "wrist deice"
Section 7.9.1: PPG is said to use "green color light". Typos "interals", "Wrisband", "finnish"
Section 9.3 Weird line break

### Aino ECG Master Design Transfer Plan
OK with the changes but more information about the actual details (eg. what "has been agreed") need to be added in the next version to all sections. Also the "shall" points need to be converted to what was actually done. Links to the documents where those are detailed is also enough.

## Demo product

- Lis???? dokumentin nimeen AMS-1 ja voisi my??s laittaa kaikki alkukirjaimet isolla, kuten on tapana
- T??yt?? etusivun tyhj??t kent??t ja roolit (koska lukee name & role)
- Kappale 2: Pit????k?? mainita jotain datan omistuksesta?
- Kappale 3 (vai joku muu): Voisi lis??t?? selvennyksen, ett?? jokainen paketti sis??lt???? oman k??ytt??j??n ja oman organisaation
- Kappale 4: Lis???? Windows version (10?) ja selain, joka asetetaan oletukseksi (Edge?)

## Capa Procedure

Typoja: "indictes", "complince", "shal", "ba", "Competene", 
Kappale 6.3. taulukko 4 ensimm??inen rivi. Pit??isik?? lis??t?? Software Development Procedure?

## AMS-1 Operations Manual

Lis???? seuraavaan versioon:
- k??ytt??jien poistaminen/muuttaminen
- asiakkuuden lopettaminen


6.3.3 The ISO and and BSI standards/certifications should be added to the references and referred in the text
8 "High availability can be achieved" --> If I were a customer I'd wonder if "Is it achieved?"
9 The IEC guidance document should be added to the references (??3) and referred in the text. Same for AES standard

### 0.16



## Aino ECG Factory tester Qualification Plan and Report

Pidet????nk?? t??t?? koko tuotantotestauksen kelpoistuksen yl??tason dokumenttina vai pit??isik?? laatia ihan oma yhteenvetodokumentti? Haluaisin, ett?? jossain selvennet????n mit?? kaikkia vaatimuksia tuotantotestaukselle on (ilmeisesti ainakin PODMS-1378432600-5350, PODMS-477950017-5515, PODMS-477950017-5606?), mitk?? testerit toteuttavat mitk??kin vaatimukset ja miten  eri vaatimusten/testereiden kelpoistus on jaettu eri dokumentteihin.
Esimerkiksi vaikuttaa, ett?? Aino ECG Factory Tester Modules Requirement Specification m????rittelee vaatimuksia, joista AinoTester2 t??ytt???? osan. AinoTester2 t??ytt??vien vaatimusten kelpoistus on ilmeisesti jaettu Aino ECG Factory Tester GW part Qualification plan and report ja Aino ECG Factory Tester Modules Qualification plan and report dokumentteihin. Osittain vaikuttaa, ett?? vaatimuksen ja testin linkitys on ID:n avulla, vaatimuksen ID on my??s testin ID. T??m?? on v??h??n h??m????v???? itse testille voisi keksi?? on 
Joku taulukko n??ist?? linkityksist?? antaisi edes jonkinlaisen mahdollisuuden todeta, ett?? kaikki vaatimukset on t??ytetty 

Onko kaikki vaatimusdokumentit p??ivitetty ajantasalle? Ent??s Aino ECG Factory Tester Version Information?

1. T??ss?? pit??isi selvent???? mihin vaatimuksiin ja testeriin t??m?? kelpoistus liittyy.
2. T??h??n pit??isi listata vaatimusdokumentit, jonka perusteella testataan. Onko t??ss?? tapauksessa pelk??st????n Aino ECG Factory Tests Requirement Specification?
4. T??h??n pit??isi listata mit?? testereit?? kelpoistus koskee ja kerrata mit?? vaatimuksia vastaan t??ss?? testataan.
6. Testeiss?? pit??isi kertoa mill?? testerill?? se on suoritettu, jos useita. Kaikille testeille ei l??ydy vaatimusta, esim G0.1.
8. Kannattaako t??t?? hyv??ksy?? edes t??ss?? vaiheessa, jos joku testi pit???? kuitenkin toistaa?


## Design change label material

Musta Jarin kuuluisi olla katselmoija.
Pit??isik?? kappaleessa 2.4 ehdotukseen sis??llytt???? my??s toimittajan vaihdos?
Kappaleessa 3.2 mulla ainakin her???? kysymys, ett?? eik?? voi mitenk????n vaikuttaa bioyhteensopivuusriskiin?

Sitten samassa kohdassa tai vasta B-osassa todetaan vaikka ett?? my??s uuden toimittajan materiaalit l??ytyy UL:n listalta linkkeineen. -> samaa materiaalia eri tuotenimi -> ei muutoksia bioyhteensopivuusriskiin.


## Aino ECG Instructions for Batch release

Poista kommentit dokumentista.
Kappaleessa 9. suluissa oleva dokumentin nimi ei ole niin selke?? tapa. Muutaisin samaan tyyliin kuin kappaleessa 10. eli Report file is xxxxx.
Muuta kappaleiden 10 ja 11 nimet samaan tyyliin kuin kappale 9.

## Aino ECG Production Description B3

Sections 5 and 6: Should the version number of each document be specified so we know the whole process for B3? This is also related to the FDA discussion.

Section 9.2 sentence "When the production has been successfully transferred to the manufacturer" is weird in this context. The design transfer has occurred a long time ago so I doesn't need to be mentioned here with batch 3.

Section 12.1 It was quite hard for me to understand the point about not marked serial numbers in the database. Maybe reformulate this to something like: Due to a human error the serial numbers of some boards that were reworked during the AOI phase were not recorded in the rework database.


## Aino ECG Production Description B4 onwards v1.8

Kommentit
- 9.2 Tuo kohta "When the production has been successfully transferred to the manufacturer" on v??h??n hassu, koska t??ss?? jo tehd????n batchia 4 ja eteenp??in jolloin tietenkin design transfer on jo tehty.
- 9.3, 9.4, 9.5: Kannattaako sales boxien sis??lt??j?? laittaa t??h??n vai vaan viitata dokkareihin, josta se l??ytyy? Mulle sopii n??inkin, mutta jos muuttuu tai tulee uusia, niin pit???? sitten t??m??kin muistaa p??ivitt????.
- 9.3: Batch release kohdassa voisi viitata PODMS-1378432600-7802 Aino ECG Instructions for Batch release -dokumenttiin.
- 11.1: Lis???? viittaus akkujen vuosihuoltoon ja tarkenna mit?? much longer than one year tarkoittaa (tarkennus voi olla tuossa vuosihuolto-oppaassa).
- 12.1: Onko B4> laitteissa edelleen tehty tuota "Unfortunate human error"?
- 12.2 ja 12.3: Kuulostaa, ett?? nuo "separate guidance" ja "Separate emails" pit??isi olla tallennettu SharePointiin


## Aino ECG Production Description B4 onwards v1.11
- Kappale 5: Virheellinen dokumentti-ID POMDS-1378432600-7802
- Kappale 9.2: typo "changeling". En oikein ymm??rr?? mit?? viimeinen lause "At the end of the production the production batch released before it was stored into the warehouse or delivered to the customer" sanoo.
- Kappale 12.1: Eik?? t??m?? ole kuvaus miten tehd????n my??s jatkossa batchien osalta? Tuo "were marked" muoto on siin?? mieless?? v????r??.


## Aino ECG Instructions for Batch release v1.3.

- Dokumentin nimess?? voisi k??ytt???? isoja kirjaimia johdonmukaisesti eli nimen muuttaa "Aino ECG Instructions for Batch Release"
- Lis???? kappaleeseen 12.3 selvennyst??, ett?? kyseess?? on Jira taski AMS-1 Operations projektissa
- Lis???? sopivaan kohtaan linkki k??ytettyyn Jira projektiin https://pulseon.atlassian.net/browse/AMS1OPS

## AMS-1 Software Security

Minusta kuvauksesta ei k??y ilmi, mit?? tietoja potilaasta ja ammattilaisesta tallennetaan j??rjestelm????n. T??ss?? etenkin henkil??tiedot tai tiedot, joilla voidaan tunnistaa henkil??.
- Lis??tty kappale 6

Web-k??ytt??liittym?? on ilmeisesti ainoastaan ammattilaisen k??yt??ss??. Miten ammattilainen saa k??ytt??oikeudet, mit?? tietoja ammattilaisesta kirjataan tunnukseen ja miten k??ytt??j??tunnistaminen toteutetaan. K??ytt??oikeustasot taisi olla.
- Tietoja lis??tty kappaleeseen 7. 

Mainitaan, ett?? j??rjestelm??n tietokanta on salattu, mutta salausavaimen hallinnasta ei ole kuvausta.
- Muutama selvennys lis??tty kappaleeseen 8.



