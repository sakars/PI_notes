# Ko var testēt statiski?

>[!info] TL;DR
>Visa veida dokumentus

- Biznesa, funkcionālās, drošības prasības
- Epiki, lietotāju stāsti, akceptēšanas kritēriji
- Arhitektūras un projektējuma specifikācijas
- Kods
- Testa programmatūru *(testware)*, iekļaujot testēšanas plānus, testu gadījumus, automatizētos testu skriptus
- Lietotāja rokasgrāmatas
- Līgumi, projekta plāni, laika grafiki un budžeta plāni
- Programmatūras, infrastruktūras konfigurācija
- Aktivitāšu diagrammas u.c. veidu diagrammas

# Statiskās testēšanas mērķi
- Identificēt un labot [[Definīcijas#Defekts (Defect)|defektus]] pirms [[Dinamiskā testēšana|dinamiskās testēšanas]]
- Identificēt un atrast [[Definīcijas#Defekts (Defect)|defektus]], kuru atrašana ar [[Dinamiskā testēšana|dinamisko testēšanu]] ir grūtāka
- Projektēšanas un kodēšanas [[Definīcijas#Defekts (Defect)|defektu]] novēršana, atklājot neskaidrības, neatbilstības, pretrunas, neprecizitātes, dublēšanos
- Izstrādes produktivitātes paaugstināšana caur projektējuma uzlabošanu
- Izmaksu un izstrādes laika samazināšana
- Izmaksu samazināšana programmatūras dzīves cikla laikā
- Komunikācijas uzlabošana starp komandas dalībniekiem

# Priekšrocības

Ir lētāk atrast un novērst
- Prasību, Projektējuma, Koda [[Definīcijas#Defekts (Defect)|defektus]]
- Novirzes no standartiem
- Nekorektas saskarnes specifikācijas
- Drošības ievainojamības
- Testu bāzes nepilnības

Lielāko daļu uzturēšanas defektu var atrast ar statisko testēšanu:
- Koda modularizācija
- Koda atkalizmantošana,
- Koda analizēšana

# Metodes
Statisko testēšanu var veiktL
- **Manuāli**, veicot [[Definīcijas#Apskate (Review)|apskates]] procesu
- **Automātiski**, veicot testēšanu ar rīku palīdzību *(static analysis)*
# Apskates

Neatkarīgi no apskates veida, vienmēr jāsagatavojas pēc iespējas vairāk.

## Apskates process
- Plānošana
- Uzsākšana
- Individuāla apskate (individuālā sagatavošanās)
- Problēmu komunicēšana un analīze
- Labošana un ziņošana

## Plānošana
- Tvēruma *(scope)* definēšana (apskates mērķis, apskates dokumenti, novērtējamie kvalitātes raksturlielumi)
- Darba un laika rāmja novērtēšana
- Apskates raksturlielumu identificēšana (apskates tips, iesaistītās lomas, veicamās aktivitātes, kontrolsaraksti)
- Iesaistīto Personu identificēšana un lomu sadale
- Ieejas un izejas kritēriju noteikšana formālākiem apskates veidiem
- Pārbauda, vai ir izpildījušies ieejas kritēriji ([[Kvalitātes pārvaldība#Formālas tehniskās apskates|Formālu apskatu]] veidiem)

## Uzsākšana
- Darba produktu izdale
- Tvēruma, mērķu, procesa, lomu un darba produktu skaidrošana dalībniekiem
- Atbildes uz iesaistīto personu jautājumiem par apskati

## Individuāla apskate
- visa vai daļēja produkta apskate
- Potenciālo defektu, rekomendāciju jautājumu atzīmēšana

## Problēmu komunicēšana un analīze
- Potenciālo defektu komunicēšana (apskates sanāksmes)
- Potenciālo defektu analīze (statusa un atbildīgā norādīšana)
- Kvalitātes raksturlielumu novērtēšana un dokumentēšana
- Identificēto vienumu novērtēšana pret izejas kritērijiem, lai pieņemtu apskates lēmumu

## Labošana un ziņošana
- Defektu ziņojuma sagatavošana par identificētajiem vienumiem, kam nepieciešamas izmaiņas darba produktā.
- Atklāto defektu novēršana apskates darba produktā (parasti veic produkta autors)
- Defektu paziņošana atbilstošajai personai vai komandai
- Defektu statusu atjaunošana (formālās apskatēs)
- Pārliecinās par izejas kritēriju izpildi (formālās apskatēs)
- Darba produkta apstiprināšana, ja ir sasniegti izejas kritēriji


## Lomas un pienākumi

### Formālās apskatēs
- Autors *(author)* - Izstrādā apskates darba produktu. Labo apskatē atrastos defektus.
- Vadība *(management)* - Atbild par apskates plānošanu, apskates izpildes lēmumu pieņemšana, piešķir cilvēku, finanšu, laika resursus, uzrauga izmaksu efektivitāti, neadekvātu rezultātu gadījumā izpilda kontroles lēmumus
- Moderators *(facilitator/moderator)* - nodrošina efektīvu apskates sanāksmju norisi, darbojas kā starpnieks dažādu viedokļu gadījumā, bieži persona no kuras atkarīgs veiksmīgas apskates iznākums.
- Apskates vadītājs *(review leader)* - Uzņemas vispārēju atbildību par apskati, nolemj par personu iesaisti apskatē.
- Apskatītāji *(reviewers)*
- Protokolētājs *(scribe/recorder)* - Salīdzina individuālās apskates laikā konstatētos potenciālos defektus. Apskates sanāksmēs pieraksta jaunus potenciālos defektus, atvērtos jautājumus un pieņemtos lēmumus.

Atsevišķi apskates tipi ļauj pieņemt vienai personai vairākus tipus. 
Lomu uzdevumi atšķiras dažādiem apskates tipiem. 
Elektroniskie rīki var aizstāt protokolētāju.

## Apskašu tipi

![[Definīcijas#Neformālā apskate (Informal review)|]]

![[Definīcijas#Caurskatīšana (Walkthrough)]]

![[Definīcijas#Formālā tehniskā apskate (FTR – Formal technical review)|D]]

![[Definīcijas#Programmas inspekcija|D]]
