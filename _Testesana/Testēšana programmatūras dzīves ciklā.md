![[Definīcijas#Tests (Test)|D]]

![[Definīcijas#Testa gadījums (Test case)|D]]

![[Definīcijas#Testa scenārijs (Test scenario)|D]]

# Testa scenārijs vs Testa gadījums


| Testa scenārijs                                                        | Testa gadījums                                                                                    |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| Augsta līmeņa dokuments, kas apraksta testējamo funkcionalitāti        | Testa gadījumi satur konkrētas darbības, datus, sagaidāmos rezultātus programmatūras testēšanai   |
| "Ko testēt?"                                                           | "Kā testēt?"                                                                                      |
| Testa scenārijs ir viena rindiņa. Var radīt neskaidrības, pārpratumus. | Norādīti konkrēti izpildes soļi, priekšnosacījumi, sagaidāmie rezultāti.                          |
| Veido no prasību dokumentācijas, lietotāju stāstiem                    | Testa gadījuma pamatā ir testa scenārijs. No viena testa scenārija veido vairākus testa gadījumus |
| Augsta līmeņa                                                          | Zema līmeņa                                                                                       |
| Palīdz ātri notestēt funkcionalitāti                                   | Palīdz detalizēti notestēt funkcionalitāti                                                        |
| Izveide ir vieglāka un ātrāka, prasa mazāk resursu.                    | Izveidei vajag vairāk resursu, jo vajadzīga dokumentācija un izpilde.                             |
| ![[Pasted image 20240421110651.png]]                                   | ![[Pasted image 20240421110359.png]]                                                              |

# Testa izpilde

Faktori kas jāņem vērā:
- Jāņem vērā risku (???), izvēloties izpildāmā testa komplekta apakškopu
- Testu gadījumu piešķiršana testētājiem
- Testu izpilde, defektu ziņošana, testu statusu uzturēšana
- Bloķējošo problēmu novēršana
- Statusu ziņošana, piešķirto testēšanas uzdevumu, plānu, prioritāšu pārskatīšana
- Testēšanas iterācijas rezultātu, statusu ziņošana

# Testēšanas plāns

Testēšanas plāns ir dokuments, kas apraksta:
- Testēšanas stratēģiju
- Mērķus
- Laika grafiku
- Novērtējumu (riski, problēmu izsekošana un ziņošana)
- Nodevums
- Testēšanai nepieciešamos resursus (testētāji, vides, tehniskais nodrošinājums)

Tas nodrošina organizētu un efektīvu testēšanas procesu, ko uzrauga un kontrolē testēšanas vadītājs.

![[Pasted image 20240421112556.png]]

![[Pasted image 20240421112544.png]]

# Programmatūras izstrādes dzīves cikls

![[Pasted image 20240421112901.png]]
- Problēmas identificēšana
- Plānošana
- Prasību analīze
- Projektēšana
- Izstrāde
- Testēšana
- Piegāde
- Uzturēšana

>[!tip]- Humoriņš
>![[Humoriņi#Plāns vs realitāte]]

Testētājam ir jāpārzina izplatītākos programmatūras izstrādes dzīves cikla modeļus.
Katrai izstrādes aktivitātei ir atbilstoša testēšanas aktivitāte.
Katram testēšanas līmenim ir specifisks testēšanas mērķis.
Testu analīze un projektēšana tiek uzsākta līdz ar attiecīgo izstrādi.
Testētāji iesaistās prasību un projektējuma precizēšanā. Piedalās arī darba produktu caurskatīšanā.
Neatkarīgi no modeļa, testēšanu jāuzsāk jau sākumposmā.

# Ūdenskrituma modelis

![[Pasted image 20240421113343.png]]


# V-modelis

![[Pasted image 20240421113411.png]]

# Iteratīvais modelis

![[Pasted image 20240421113431.png]]

# Spējās pieejas modelis (Agile)

Skatīt [[Definīcijas#Spējā izstrāde (Agile)]]

![[Pasted image 20240421113456.png]]

# Modeļu iedalījums

Pēc ISTQB iedala:
- **Secīgie** modeļi (ūdenskrituma, V-modeļa)
- **Iteratīvie**, **Inkrementālie** modeļi (ar katru reizi labāks)

## Secīgās izstrādes modeļi
- **Ūdenskrituma modelis**
- **V-modelis**

## Iteratīvās izstrādes modeļi
- Spējā izstrāde *(Agile)*
	- RUP *(The Rational Unified Process)* - garākas 2-3 mēn. iterācijas ar apjomīgākām piegādēm
	- Scrum - īsas iterācijas (stundas, dienas vai dažas nedēļas) ar neliela apjoma piegādēm
	- Kanban - nenoteikta vai noteikta garuma iterācijas ar vienu uzlabojumu vai vairāku uzlabojumu apvienojumu piegādi

# Modeļu konteksts

Modeli izvēlies atbilstoši projektam un mērķiem.

Atkarībā no projekta var nākties kombinēt, reorganizēt testēšanas līmeņus un/vai aktivitātes.

Dažādus modeļus var kombinēt dažādām produkta daļām (V-modelis aizmugursistēmai, Spējais priekšgala sistēmai)

Iemesli pielāgot programmēšanas dzīves cikla pielāgošanai projekta kontekstam:
- Sistēmu produktu risku atšķirības (sarežģīts vai vienkāršs projekts)
- Daudzas biznesa vienības var būt daļa no projekta vai programmas (secīgas un spējās izstrādes kombinācija)
- Īss laiks produkta piegādei

# Testēšanas līmeņi

1. Vienībtestēšana - viena komponente vai funkcija - veic programmētājs
2. Integrācijas testēšana - savieto komponentes - veic testētājs
3. Sistēmas testēšana - visa sistēma kopumā - veic testētājs
4. Akcepttestēšana - vai sistēma atbilst vēlmēm - veic lietotājs


# Testēšanas līmeņu raksturlielumi
- Mērķis
- Testu bāze testu gadījumu izstrādei
- Testējamias objekts
- Tipiskie defekti un kļūmes/atteices
- Pieejas un atbildības
- Testēšanas vides

# Verifikācija vs Validācija

![[Pasted image 20240421132811.png]]
![[Definīcijas#Verifikācija (Verification)|D]]

![[Definīcijas#Validācija (Validation)|D]]

# Testēšanas tipi

- Funkcionālā
- Nefunkcionālā
- Baltās kastes
- Izmaiņu saistīta

## Funkcionālā
Notestē kas jādara sistēmai un vai izdara visu kas minēts prasībās.

## Nefunkcionālā
Notestē cik labi sistēma darbojas.
Testē nefunkcionālās prasības.
Jātestē visos līmeņos jo nefunkcionālās problēmas izlabot vajag agri


## Baltās kastes testēšana

Pārbauda iekšējo darbību.

Pārklājums pēc tā, cik liela daļa koda tiek izpildīta.

## Izmaiņu saistīta testēšana

Pēc izmaiņas jāveic:
- **Apstiprināšanas testēšana.** Pēc defekta novēršanas jāpārtestē visu kas neizpildījās.
- **Regresā testēšana.** Jāpārtestē visu pārējo, vai kkas cits netika salauzts.

Abas jāpilda visos testēšanas līmeņos.
Varētu noderēt sataisīt regresos testus automātiski.

# Uzturēšanas posms

Uzturēšanā jāturpina uzturēt nefunkcionālo kvalitātes kritēriju izpildi: veiktspēju, savietojamību, uzticamību, drošību u.c.

Jānodrošina platformu, datu migrācija

# Uzturēšanas ietekmes analīze

Jānovērtē sistēmas izmaiņas, lai identificētu:
- Iespējamās sekas
- Paredzamās izmaiņu blakusparādības
- Sistēmas apgabalus, uz kuriem ir ietekme
- Izmaiņu ietekmi uz testiem

Analīzi sarežģī:
- novecojusi dokumentācija
- Testa gadījumi nav dokumentēti vai ir novecojuši
- Netiek nodrošināta, uzturēšana trasējamība starp testiem un testu bāzi
- Vājš rīku atbalsts
- Netiek veltīta uzmanība uzturēšanai