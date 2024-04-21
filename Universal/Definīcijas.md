---
aliases:
  - D
---

#definīcijas
# A

## Ad hoc
[[#Apskate (Review)|Apskates]] tehnika, kurā apskatītājiem dod maz vai nedod nemaz informāciju par veicamo uzdevumu
Apskatītāji izskata dokumentāciju secīgi un dokumentē identificētās problēmas
To lieto, kad nav nepieciešama vai nepieciešama neliela sagatavošanās.
Rezultāts atkarīgs no apskatītāju prasmēm un zināšanām.
Var veidoties ziņoto problēmu dublikāti.

## Apskate (Review)

Process, kurā kādu darba produktu (dokumentāciju, komponentes dizainu, komponentes kodu) izvērtē pēc zināmām kvalitātes prasībām un atrod [[#Defekts|defektus]].

Skatīt [[Kvalitātes pārvaldība#Apskates un inspekcijas (Reviews and inspections)]], [[Statiskā testēšana#Apskates]]


## Atkļūdošana (debugging)

Izstrādes aktivitāte, ar kuras palīdzību atrod, analizē, labo sistēmas [[#Defekts (Defect)|defektus]]

## Atteice (Failure)

Programmatūra nedarbojas kā paredzēts dažādu iemeslu dēļ.
Arī [[#Kļūme (Failure)]], [[#Incidents (failure)]]
# Ā

# B

## Baltās kastes testēšana (White-box tests)

Testēšana, kura testē to, kā modulis strādā (zinot iekšējās darbības) jeb kvalitatīvus testus.

Pretējais [[#Melnās kastes testēšana (Black-box testing)|Melnās kastes testēšanai]]


# C
## CASE
**C**omputer **A**ided **S**oftware **E**ngineering
jeb programmatūras izstrāde ar datora palīdzību.
**CASE tools** - programmatūras rīki, kas palīdz izstrādei.

## Caurskatīšana (Walkthrough)
[[#Apskate (Review)|Apskates]] veids.
- Mērķi: atrast defektus, uzlabot produktu, apsvērt alternatīvas.
- Individuālā apskate nav obligāta.
- Var veikt scenāriju izpildes, simulācijas, "sausās izpildes" *(dry run)*
- Potenciālo defektu žurnalēšana
- Kaut kas starp neformālu un ļoti formālu apskati

## Cēlonis (Root cause)

Darbība, kas izraisīja [[#Defekts (Defect)|defektu]]: nepareiza sintakse kodā, nepareizu vērtību izmantošana u.c.

## Cēloņu analīze (Root cause analysis)

[[#Cēlonis (Root cause)|Cēloņa]] izmeklēšana, analīze, lai novērstu turpmāku problēmas atkārtošanos.
## CMM (Capability maturity model)

Modelis, kas raksturo programmatūras briedumu pēc tā spējām.

Skatīt:
- [[Kvalitātes pārvaldība#Programmatūras kvalitāte un CMM (Capability Maturity Model)]]
- [[CMM Metriku definīcijas standarts]]




## COCOMO

**COCOMO** (**CO**nstructive **CO**st **MO**del) jeb konstruktīvais izmaksu modelis (?) ir regresijas models, kas balstīts uz koda rindu skaita.

Šis modelis ir labi piemērots uzticamai izmaksu, laika, apjoma un darbietilpības un kvalitātes aprēķināšanai.

To oriģināli izveidoja Berijs Boēms (Barry Bohem) 1981. gadā. Tas ir balstīts uz 63 projektu pētījumu, kas to padara par vienu no vislabāk dokumentētajiem modeļiem.

Skatīt [[Darbietilpība#COCOMO]]

# Č

# D
## Darbietilpība (Effort)

Darbietilpība (Effort) ir strādāšanas daudzums, kas vajadzīgs, lai pabeigtu [[Definīcijas#Darbs/Aktivitāte (Activity/Task)|darbu]]. To parasti mēra [[#Persondiena/Personmēnesis (Person-days/Person-months)|personlaikā]].

Parasti darbietilpību vienādojumos apzīmē ar $E$

## Darbs/Aktivitāte (Activity/Task)

Aktivitāte jeb darbs ir vismazākais plānošanas elements

## DCI (Data Collection Item)

Informācijas vienība, kuru izmanto mērījumiem.

Skatīt:
- [[CMM Metriku definīcijas standarts]]
- [[Programmatūras mērīšana]]

## Defekts (Defect)

[[#Apskate (Review)|Apskatē]] vai testēšanā atrasta problēma kodā.

## Dinamiskā testēšana (Dynamic testing)

[[#Testēšana (Testing)|Programmatūras testēšana]], izpildot programmatūras kodu.

Skatīt [[Dinamiskā testēšana]], [[#Statiskā testēšana (static testing)]]

## Dūmu testēšana (smoke test)

Pārliecinās, vai programmatūras kritiskā funkcionalitāte darbojas
- Pārbauda sistēmas stabilitāti
- Pārbauda/izpilda visu sistēmu
- Ir kā vispārējā veselības pārbaude

# E

## Ekstrēmā programmēšana (XP or eXtreme Programming)

[[#Spējā izstrāde (Agile)|Spējās izstrādes]] ietvars, kas specializējas ar īpaši ātru izstrādes ciklu un [[#Pāru programmēšana (Pair programming)|pāru izstrādi]].

[Extreme programming - Wikipedia](https://en.wikipedia.org/wiki/Extreme_programming)

# Ē

# F

## Fan-in/Fan-out

Pieņemam kādu funkciju X.

Funkcijas X _Fan-in_ ir skaits, cik funkcijas izsauc X

Funkcijas X _Fan-out_ ir skaits, cik funkciju izsauc funkcija X.

Liels Fan-in nozīmē, ka X ir cieši saistīta ar sistēmu un tās mainīšana stipri ietekmē sistēmmu.

Liels Fan-out nozīmē, ka iespējams X ir pārāk sarežģīta un to būtu jādala sīkāk.




## Funkcionālie punkti (Function points)

Funkcionālie punkti ir mērvienība, kas apzīmē konkrētu daudzumu funkcionalitātes. Tas ir viens no veidiem kā prognozēt [[#Darbietilpība (Effort)|darbietilpību]]. 

## Formālā tehniskā apskate (FTR – Formal technical review)

Formāla [[#Apskate (Review)|apskate]], kurā apspriež kādu produktu.

Mērķi:
- Panākt vienprātību, potenciālo defektu identificēšana
- Kvalitātes novērtēšana
- Ideju ģenerēšana
- Alternatīvu novērtēšana

Individuālā apskate ir obligāta.
Protokolētājs ir obligāts
Potenciālo defektu žurnālu un apskates ziņojumu izveide.

Skatīt [[Kvalitātes pārvaldība#Formālas tehniskās apskates]]




# G

# Ģ

# H

# I

## Incidents (Failure)

![[#Atteice (Failure)]]


# Ī

# J

# K

## Kļūda (Error)

Cilvēka (tipiski programmētāja) darbības vai lēmuma rezultātā radīts nekorekts, negaidīts rezultāts.
Cilvēks kļūdas, rakstot kodu vai dokumentu.

## Kļūdaini negatīvs (False negative)

[[#Kļūme (Failure)|Kļūme]], kas tika palaista garām.
## Kļūdaini pozitīvs (False positive)

Atrasta [[#Kļūme (Failure)|kļūme]], kur īstenībā kļūmes nav.

## Kļūme (Failure)

![[#Atteice (Failure)]]

## Kontrolsaraksti
Sistemātiska tipisko defektu tipu pārbaude.
Sastāv no jautājumiem, kas balstīti uz iepriekšējo pieredzi.
Tiek veidoti atbilstoši apskatāmā darba produkta tipam.
Tiek atjaunoti ar agrāk nepamanītiem defektiem.
Svarīgi identificēt defektus, kas nav iekļauti kontrolsarakstā.

## Kvalitātes apskate (Quality review)

[[#Apskate (Review)|Apskate]] kurā cilvēku grupa uzmanīgi pārskata daļu vai visu programmatūru un dokumentāciju, kas ar to saistīta.
Apskatīt var kodu, dizainu, specifikācijas, testa plānus, standartus u.c.
Tos var "parakstīt" apskatē, kas norāda progresa stadijas apstiprinājumu no pārvaldības.

Skatīt [[Kvalitātes pārvaldība#Apskates un inspekcijas (Reviews and inspections)]]

## Kvalitātes dokumentācija (Quality documentation)

[[Kvalitātes pārvaldība|Kvalitātes pārvaldībā]] izmantots progresa un izstrādi aprakstošs saraksts, kas atbalsta izstrādes procesu izstrādes komandas sastāva maiņas gadījumā. 
## Kvalitātes kontrole (Quality control)

[[#Kvalitātes nodrošināšana (Quality assurance)|Kvalitātes  nodrošināšanā]] definēto procesu un standartu **pielietošana**, lai filtrētu produktus, kas neatbilst prasītajai kvalitātei.

Nesajaukt ar [[#Kvalitātes nodrošināšana (Quality assurance)]]
Skatīt [[Kvalitātes pārvaldība]]
## Kvalitātes nodrošināšana (Quality assurance)

### PI definīcija
Procesi un standarti, kuriem *vajadzētu* rezultēties augstas kvalitātes produktos, kā arī šo procesu un standartu ieviešana izstrādes procesā.

Nesajaukt ar [[#Kvalitātes kontrole (Quality control)]]
Skatīt [[Kvalitātes pārvaldība]]

### PT definīcija
Sistemātisks process, lai noteiktu vai produkts vai pakalpojums atbilst noteiktām prasībām un piemērots paredzētajiem mērķiem. Ietver visu izstrādes procesu un nodrošina, ka katrs produkta aspekts ir kvalitatīvs.

Skatīt [[Kvalitātes nodrošināšana un testēšana]]
# Ķ

# L

## Laikplānošana (Scheduling)

Laikplānošana ir process kā sadalīt darbu sīkāk un kā un kad šie sīkie darbi tiks izpildīti.

Skatīt [[Projektu plānošana#Laikplānošana]]
## Laikplāns (Schedule)

Laiks, kas apzīmē darbiem vajadzīgo laiku vai saraksts, kas satur visus vajadzīgos darbus. Parasti šo laiku mēra nedēļās, mēnešos vai retāk gados.

# Ļ

# M

## Melnās kastes testēšana (Black-box testing)

Testēšanas veids, kurā pārbauda moduļa darbību, nezinot kā tas strādā. Šie testi ir kvantitatīvi.

Pretējais [[#Baltās kastes testēšana (White-box tests)|Baltās kastes testēšanai]]

## Metrika (Software metric)

Mērījuma veids, kas saistīts ar programmatūru, procesu vai dokumentāciju.
Piem. [[#Pirmkoda rindas (Lines Of Code) (LOC)]], Fog indekss, [[#Darbietilpība (Effort)]]

Skat. [[Programmatūras mērīšana]]
# N

## Neformālā apskate (Informal review)

Neformāla [[#Apskate (Review)|apskate]], kas iekļauj mazāk plānošanas nekā [[#Formālā tehniskā apskate (FTR – Formal technical review)|formālai tehniskajai apskatei]]. Tās mērķis ir iegūt citu viedokļus bez smagas dokumentēšanas un birokrātijas.
To izmanto arī risinājumu, ideju ģenerēšanai, nelielu problēmu risināšanai.

Rezultāti var tikt dokumentēti.
Bieži izmanto [[#Spējā izstrāde (Agile)|spējās izstrādes]] dzīves cikla laikā.

Skatīt [[Kvalitātes pārvaldība#Neformālās apskates]]

## Nodevumi (Deliverables)

Produkti, kurus atdod klientam, piemēram, prasību dokuments sistēmai.

# Ņ

# O

# P

## Paraugu virzīta apskate (SDR – Sample-Driven Review)

[[#Apskate (Review)|Apskates]] veids, kurā cenšas kvantificēt tos darba produktus, kuriem parasti veiktu [[#Formālā tehniskā apskate (FTR – Formal technical review)|formālu tehnisko apskati]]

Tās pamatā ir paņemt mazu daļu $a$ no katra produkta $i$. 

No tiem pieraksta kļūdu skaitu $f_i$ katrā $a_i$.

Veido groza prognozi (gross estimate) kļūdām produktā $F_i = \frac{f_i}{a_i}$

Sakārto produktus dilstošā secībā pēc kļūdu groza prognozes.

Virzīt resursus uz tiem produktiem, kuriem ir lielākās prognozētās problēmas.

Skatīt [[Kvalitātes pārvaldība#Apskates un inspekcijas (Reviews and inspections)]]

## Pareizības testēšana (sanity test)

Pārbauda vai visas kļūdas ir novērstas pēc būvējuma izveidošanas
- Pārbauda piegādes racionalitāti, lai turpinātu ar stingrākiem testiem
- Pārbauda/izpilda konkrētu sistēmas komponentu
- Ir kā specializēta veselības pārbaude
## Pāru programmēšana (Pair programming)

Programmēšanas veids, kurā programmē vienlaicīgi 2 cilvēki pie viena datora. Viens raksta kodu, otrs pārlūko uzrakstīto un izsaka ieteikumus. Pēc kāda laika abi apmainās.

Šī metode dod priekšrocību, ka kļūdas var tikt atrastas ātrāk un tādējādi tiek uzlabota produkta kvalitāte.

Procesā abi programmētāji gūst saprašanu par konkrēto koda daļu, kas uzlabo komandas vienotību un samazina problēmas.

Šī metode palīdz atrast problēmas, kuras ir gandrīz neiespējami atrast inspekcijās.

Taču tai ir arī mīnusi:
- Kopīgas nesaprašanās – abi izstrādātāji var pārprast specifikāciju un diskusija var novērst pie pārpratuma stiprināšanās
- Pāru reputācija – reputācijas saglabāšanas nolūkos pāri var negribēt meklēt kļūdas kodā, lai nepalēlinātu progresu
- Darba attiecības – pāri var satuvināties, kas var novest pie vājinātas kritikas, lai nesabojātu attiecības


## Persondiena/Personmēnesis (Person-days/Person-months)
Mērvienība, kas apraksta [[#Darbietilpība (Effort)|darbietilpību]]. Tā apzīmē darbu, ko noteikts daudzums cilvēku var paveikt noteiktā laikā.

> [!warning] Uzmanību
> Cilvēku daudzums nav proporcionāls darbam (skatīt [[Humoriņi#Freda Bruksa likums (Fred Brooks' law)|humoriņu]]), taču parasti šo mērvienību izmanto [[Darbietilpība#Empīriskie modeļi|empīrisku modeļu]] formulās. 

## Pirmkoda rindas (Lines Of Code) (LOC)

Apjoma mērvienība, kas rindu skaitu pirmkodā. Lielus projektus mēra kilorindās (KLOC)

Saīsina arī uz SLOC (source lines of code)


## Procesa standarti (Process standards)

Procesa standarti ir standarti, kas attiecināmi uz izstrādes procesiem, pie kuriem jāpieturas izstrādes laikā. 
Tie iekļauj:
- specifikācijas
- dizainus
- validēšanas procesus
- atbalsta rīkus
- dokumentus, kurus izstrādes laikā jāveido

Skat. [[Kvalitātes pārvaldība#Programmatūras standarti]]

## Produkta standarti (Product standards)

Produkta standarti ir standarti, kas attiecināmi uz produktu, kuru izstrādā.
- Dokumentu standarti
- Dokumentācijas standarti
- Kodēšanas standarti

Skat. [[Kvalitātes pārvaldība#Programmatūras standarti]]

## Programmas inspekcija

Tā ir biedru [[#Apskate (Review)|apskate]], kur tiek pētīts produkta avots (pirmkods, dokumenti), meklējot anomālijas vai defektus.
Tām parasti nav vajadzīga sistēmas izmantošana, līdz ar to inspekciju var veikt pirms implementācijas.
Inspekciju var veikt jebkurai sistēmu pārstāvošai daļai (prasības, dizains, [[Konfigurācijas pārvaldība|konfigurācijas]] dati, testu dati u.c.)

Mērķi:
- potenciālo defektu identificēšana
- kvalitātes novērtēšana
- produkta uzticamības celšana
- vienprātības panākšana

Obligāti:
- Konkrētas lomas
- Protokolētājs
- Vada apmācīts moderators (ne darba autors)
- Autors nedrīkst ieņemt apskates vadītāja, apskatītāja, moderatora, protokolētāja lomu
- Potenciālo defektu žurnāls un apskates ziņojumu izveide

## Programmatūra (Software)

Datoru programmas, procedūras un ar tām saistītā dokumentācija.
## Programmatūras kvalitāte (Software quality)

Programmatūras kvalitāte vienkāršoti nozīmē, ka produkts atbilst specifikācijai, taču kvalitāte ir termins, kas krasi atšķiras izstrādātājiem (atkārtota izmantojamība, uzturamība u.c.) un klientiem (veiktspēja, uzticamība u.c.)

Skatīt [[Kvalitātes pārvaldība#Programmatūras kvalitāte]]

## Programmatūras mērīšana (Software measurement)

Programmatūras mērīšanas mērķis ir aprakstīt kādu programmatūras īpašību ar skaitlisku vērtību.

Skatīt [[Programmatūras mērīšana]]


## Programmatūras standarts (Software standard)

Programmatūras standarti definē prasītās īpašības vai procesus, lai nodrošinātu programmatūras kvalitāti.

Standarti var būt dažādu līmeņu – starptautiski, nacionāli, organizatoriski, projektu.

Skatīt [[Kvalitātes pārvaldība#Programmatūras standarti]]

# Q

## QSM (Quantitative Software Management)

Pasaulē atzītākā komercsabiedrība, lai prognozētu [[#Darbietilpība (Effort)|darbietilpību]]. 


[www.qsm.com](http://www.qsm.com/)

# R
## Risks (Risk)

Risks ir potenciāls negatīvām sekām
Risks ietver iespēju par kādām sekām no darbinieku vai pārvaldnieku darbības vai bezdarbības, kas ir svarīgas cilvēkiem.

Skatīt [[Riska pārvaldība]]
## RMMM 
**R**isk **M**itigation, **M**onitoring & **M**anagement
jeb risku mazināšana, uzraudzība un pārvaldība
# S

## Scenāriji, "Sausās izpildes"
Strukturētas darba produkta lasīšanas/iepazīšanas vadlīnijas
Veic darba produkta "sauso izpildi"
Scenāriji palīdz identificēt defektus.
Svarīgi identificēt defektus, kas nav dokumentēti

## Scrum

Scrum ir [[#Spējā izstrāde (Agile)|spējās izstrādes]] ietvars, kas dala darbu daudzās daļās ar konkrētiem mērķiem un laika ierobežojumiem.

[Scrum (software development) - Wikipedia](https://en.wikipedia.org/wiki/Scrum_(software_development))

## Sekas (Effects)

_PT kontekstā_
Pēc [[#Programmatūra (Software)|programmatūras]] [[#Atteice (Failure)|atteices]] produkcijas vidē iesniedz problēmas pieteikumu vai sūdzību.
Sekas var arī būt arī darbinieka atlaišana.

Skatīt [[Ievads|Testēšana]]
## Spējā izstrāde (Agile)

Izstrādes veids, kas koncentrējas uz mazām grupām un ātriem izstrādes cikliem. Šis izstrādes veids spēj strauji pielāgoties prasību maiņām un piegādā programmatūru katra cikla beigās.

Skatīt [[Projektu plānošana#Agile (spējās izstrādes) plānošana]]


## Spējās izstrādes sprints (Agile sprint)

Īsa izstrādes iterācija, kas koncentrējas uz nākamo sistēmas izdevumu. Parasti sprints aizņem 2-4 nedēļas komandai.

## Statiskā testēšana (static testing)

[[#Testēšana (Testing)|Programmatūras testēšana]], neizpildot programmatūras kodu.

Skatīt [[Statiskā testēšana]], [[#Dinamiskā testēšana (Dynamic testing)]]

# Š
## Šķirtne (Milestone)

Punkts [[Projektu plānošana#Laikplānošana|laikplānā]] pēc kura var izvērtēt progresu, piemēram, kad iespējams nodot programmatūru testēšanai.

# T

## Testa gadījums (Test case)
Konkrēts apstākļu, mainīgo un darbību kopums, kas tiek lietots programmatūras darbības pārbaudē. Testa gadījumā norādīti:
- Priekšnosacījumi
- Pārbaudes darbības
- Testa dati
- Pēcnosacījumi

Saturs:
- identifikators
- scenārija identifikators
- prasības identifikators
- Testa apraksts
- Pieņēmumi, priekšnosacījumi
- Testa dati
- Izpildāmie soļi
- Sagaidāmais rezultāts (Pēcnosacījumi)
- Aktuālais rezultāts
- Veiksmīga/neveiksmīga izpilde *(OK/NOK)*


## Testa scenārijs (Test scenario)
Testa scenārijs, arī testa kopa
Testa gadījumu kopums, kas palīdz testēšanas komandai noteikta projekta pozitīvās un negatīvās īpašības.

Piemēri:
- Pārbaudīt meklēšanas funkcionalitāti
- Pārbaudīt maksājumu funkcionalitāti
- Pārbaudīt pieslēgšanās funkcionalitāti






## Testēšana (Testing)

1. [[#Programmatūra (Software)|Programmatūras]] un aparatūras pārbaude, izmantojot [[#Tests (Test)|testus]].
2. [[#Kvalitātes nodrošināšana (Quality assurance)|Kvalitātes nodrošināšanas]] apakškopa un attiecas uz sistēmas vai komponentu novērtēšanu ar nolūku noskaidrot, vai tās atbilst noteiktajām prasībām.

Skatīt [[Kvalitātes nodrošināšana un testēšana]]
## Tests (Test)

Standartizēts uzdevums, pēc kura izpildīšanas var pārbauīt datora vai sistēmas atbilstību paredzētajām prasībām.

## Testu bāze
Prasību specifikācijas, piemēram biznesa prasības, funkcionālās prasības sistēmas prasības, lietotāju stāsti, epiki, lietošanas gadījumi, vai citi darba produkti, kas apraksta sistēmas funkcionālo vai nefunkcionālo darbību.

Projektējuma dokumentācija

Sistēmas kods, datu bāze, vaicājumi saskarnes

Riska analīzes ziņojumi, kuros var ņemt vērā komponenta vai sistēmas aspektus.

# U
# Ū
# V
## Validācija (Validation)

Process, kurā, sadarbojoties ar klientu tiek pārbaudīta produkta atbilstība vēlmēm. Ja vēlmēm neatbilst, tad vēlmes tiek precizētas prasībās.

Notiek pēc [[#Verifikācija (Verification)|verifikācijas]]

## Veiktspēja (performance)

Rādītājs, kas norāda cik "labi" kāds cilvēks, iekārta vai programmatūra darbojas.
## Verifikācija (Verification)

Process, kurā produkts tiek pārbaudīts pret prasību specifikāciju vai konkrētā etapa sākumā definētajām prasībām.

Notiek pirms [[#Validācija (Validation)|validācijas]]

## Vienībtestēšana (Unit testing)

Programmatūras testi, kas pārbauda kāda moduļa funkcionalitāti. Parasti tie ir īsi testi, kas verificē moduļa atbilstību prasībām.

# Z
# Ž
