
![[Definīcijas#Programmatūras mērīšana (Software measurement)]]

Salīdzinot skaitliskās vērtības iespējams salīdzināt izstrādes paņēmienus un procesus.

Lai arī daži uzņēmumi ir radījuši programmas, kas spēj mērīt  programmatūru, sistemātisks izmantojums vēl nav populārs.

Arī standartu mērīšanai ir ļoti maz.

# Metrikas

![[Definīcijas#Metrika (Software metric)]]

## Metriku veidi

- Cik laika aizņēma process
- Vajadzīgie resursi procesam
- Kādas situācijas sastopamība

## Novērtētāja un kontroles mērījumi

![[Pasted image 20240118161902.png]]

## Metriku izmantojums

Metrikas galvenie izmantojumi ir:

- Dot [[Kvalitātes pārvaldība#Galvenās kvalitātes īpašības|kvalitātes īpašībām]] skaitlisku vērtību
- Identificēt komponentes, kuru kvalitāte ir zem standarta

## Pieņēmumi

Programmatūras īpašības var precīzi mērīt.

To, ko nevar mērīt, tam eksistē kāds savienojums ar to ko varam mērīt. Ne vienmēr šo savienojumu ir iespējams noteikt un izmērīt ārējās kvalitātes īpašības no iekšējām.

## Savienojumi starp iekšējām un ārējām īpašībām

![[Pasted image 20240118162633.png]]

# Mērīšanas problēmas industrijā

Ir neiespējami aplēst, cik vērtīgi ir ieviest organizatorisko metriku programmatūru.

Metrikas un procesi mērīšanai nav standartizēti.

Daudzos uzņēmumos izstrāde ir nepietiekami standartizēta un kontrolēta.

Liela daļa mērīšanas fokusējas uz plāniem balstītiem procesiem vai koda balstītām metrikām. 

Mērīšanas procesi pievieno procesiem papildu virstēriņu.

# Empīriskā programmatūras inžinierija

Metrikas un programmatūras mērīšana ir pamats empīriskajai programmatūras inžinierijai.

Šajā pētījumu jomā no reālajām metrikām un datiem veido un validē hipotēzes par dažādiem izstrādes paņēmieniem.

Šāda veida inžinierijai nav bijis ievērojams iespaids uz pielietotajām izstrādes metodēm

Ir grūti pielīdzināt pētījumus projektiem, kas krasi atšķiras no pētījumos apskatītajiem projektiem.

# Produktu metrikas

Kvalitātes metrikai būtu jāraksturo produkta kvalitāti.

Metriku veidi:
- Dinamiskās metrikas
- Statiskās metrikas

## Dinamiskās metrikas

- Ievāc programmas darbības laikā.
- Raksturo veiktspēju un uzticamību.
- Cieši saistītas ar kvalitātes īpašībām.

Piemēri:
- atbildes laiks – veiktspēja
- kļūdu skaits – uzticamība

## Statiskās metrikas

- ievāc no sistēmas atainojumiem, 
- raksturo sarežģītību, saprotamību, uzturamību
- Netieši saistītas ar kvalitātes īpašībām

Piemēram:
- [[Definīcijas#Fan-in/Fan-out|Fan-in/Fan-out]]
- [[Definīcijas#Pirmkoda rindas (Lines Of Code) (LOC)|pirmkoda rindas]]
- [Cyclomatic complexity](https://en.wikipedia.org/wiki/Cyclomatic_complexity)
- Vidējais identifikatoru garums
- Ietverto pārbaužu dziļums (?) (Depth of conditional nesting) – cik if-statementi cits citā
- [Gunning fog index](https://en.wikipedia.org/wiki/Gunning_fog_index)
- Svērtais metožu skaits uz klasi
- Mantošanas koka dziļums
- Tieši mantojošo klašu daudzums
- Savienotība starp klasēm (coupling between object classes)
- Klases atbildes indekss (?) – Cik metodes var tikt izsauktas, kad klase saņem ziņu
- Metožu kohēzija

Šīm metrikām jāatrod attiecības ar kvalitātes īpašībām kā sarežģītība, izprotamība, uzturamība.

# Komponenšu analīze

Katru sistēmas komponenti var analizēt atsevišķi izmantojot dažādas metrikas.

Metriku vērtības var salīdzināt ar dažādām komponentēm, kā arī vēsturiskiem datiem no iepriekšējiem projektiem.

Anomāli mērījumi liecina par kvalitātes problēmām komponentē.


![[Pasted image 20240123113650.png]]

# Mērījumu neskaidrība

> [!warning] Datus ir viegli pārprast

Nepietiek skatīties tikai uz datiem, jāskatās arī uz to kontekstu.

Kā piemēram, nepietiek skatīties uz kopējo atrasto kļūdu skaitu, jo kļūdas var palielināties līdz ar lietotāju skaita pieaugumu, kas nenozīmē, ka programmatūra pasliktinās.

Īpaši jāuzmanās mērījumi, kas saistīti ar cilvēkiem, jo cilvēki ir dažādi un jāraugās uz to ļoti uzmanīgi.

# Programmatūras analīze

Programmatūras analīze ar programmatūras datiem tiek veikta ar nolūku komandām gūt ieskatu no saviem datiem, kas ļautu veikt labākus lēmumus.

> [!info] Annalīzei vajag datus
> **Automatizētā datu ievākšana** no lietotājiem sniedz 
