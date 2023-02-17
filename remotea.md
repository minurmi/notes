
# Telco 28.01.2020

## Taustaa
- Coronaria on suomen suurin tarjoaja Holter mittauksille

## Tarjonta
- Smart ECG
- Data Management Service

## Platform:
- Käy on premises asennus:
    + Vaatii kolme virtuaalikonetta ja verkon niiden välille.
- On tehty asennuksia Azure, Google, AWS
- Toimii hyper-V ympäristössä:
    + HUSill vmware klusteri

## Kustomointi
- Max 2 kk, kustomointi, 2 henkilöä, Iman ja Janne Hansen
- PC clientti, joka tuuppaa pilveen

## Sairaalaintegraatio
- Apotissa toimii suoralla URLilla
- Lääkäri käyttää toimikorttia kirjaumaan koneeseen
- HUSilla active directory
- Google tai Microsoftin ID hallintaa tarjottu maailmalla
- Uniikki URL, joka sisältää lääkärin ja potilaan tiedon toimii pseudonymisoidulle datalle.


# Meeting 07.02.2020

Tech-tiimi:
- Kimmo (CTO) + 2 koodaria, kaikki ECG "domain" osaajia
    + 3, joista Heikki Jano GE:ltä
- On ollut turbulenssia tech-tiimissä
- Jos halutaan koodata kaikki, tarvitaan 5-6 peruskoodaria
- Ukrainasta ostetaan koodaustyötä
- Kimmo haluaisi, että palkataan pari lisää
- Samilla on hyvä verkosto --> saa tarvittaessa palkattua työvoimaa
- Beatscanner: SmartECG toteutettiin pelkälle sykedatalle kännykkäapille. Siihen kesti 20 000

# Perus
- 2 myyntiagenttia: Jenkit ja Lähi-itä
- Coronaria osti 40 henkilöä
- Myytiin holter ja uniapnea laitetteet Bittiumille 2018 
- 60 tuhatta lausuttua ECG tallennetta
- 3 sairaalaa, 2 pilotoi ja HUS maksaa vähän
- On tehnyt konsulttityötä

Kimmo
- RemoteAlle tulee pyyntö listätä käyttäjä
- Sähköpostilla kijaudutaan
- Lisää oman nimen ja salasanan
- Yhteydenotto adminille
- Laatuestimaatti samantien
- WFDB ja EDF tiedostomuoto
- Samaan organisaatioon kuuluville voidaan jakaa tallenne
- ID uniikki per organisaatio
- Jokaiselle oma pilvi-instanssi
- quality, events, episodes, trensds (hr, episodien määrä), selection (valitse näytteet), report
- Luokittelu ja klusteroinit (tulee eri fokuksesta sydämestä): Normal, supreventircular, ventricular, fusion unknown
- Käyttäjä voi editoida lyönnin tyyppiä
- Eteis ja kammiolisälyönnit
- Lyöntikohtainen syke tai RRI
- Episodit: normal sius thythm, supraventricual trigeminy, suptraventricular quadrigeminy
- Trendit

Ilman + Anna
- 2 min intervals for AF detection
- käyttää yhtä leadia, jota käytetään kaikissa

# 13.02.2020

CAP - Coronaria Analyysipalvelut
Terveystalo:
- MS dynamics perusjärjestelmä,
- Cardiac navigator ECG,
- Uniapnea Knox (export PDF, upload to potilaskertomus)
- Osastosihteeri on nakkikone, joka tekee manuaalisia uploadia järjestelmien välillä

Laiterekisteri
- Huoltohistoria, läheltäpiti tilanteet (HILMA), mitä potilaita on tällä mitattu

CAP: salanana + käyttäjätunnus
+ selaimeen uploadataan sertifikaatti
+ IP rajaus
+ tekstiviestivarmennus


SaaS palvelu vai sairaalan omassa pilvessä


Software architecture
