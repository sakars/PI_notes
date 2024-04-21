# Saturs
- [[#Testu organizēšana]]
- [[#Testu plānošana un novērtēšana]]
- [[#Konfigurācijas pārvaldība]]
- [[#Riski un testēšana]]
- [[#Defektu pārvaldība]]

# Testu organizēšana

## Neatkarīgā testēšana

Testēšanas līmeņi:
1. nav neatkarīgu testētāju, testētājs testē savu kodu
2. neatkarīgie testētāji projekta komandas ietvaros (kolēģi taisa testus)
3. neatkarīga testētāju komanda organizācijas ietvaros
4. vairākas testētāju komandas atšķirīgos lauciņos (lietojamība, drošība utt.)
5. neatkarīgi testētāji ārpus organizācijas

Komponentes testē izstrādātājs
Komponentu Integrāciju testē izstrādātājs
Sistēmu un sistēmas integrāciju testē neatkarīga komanda
Akcepttestēšanu veic pasūtītāja biznesa analītiķis vai nozares eksperts

### Plusi
- atklāj atšķirīgus defektus no testētājiem
- neatkarīgi testētāji verificē, apstrīd pieņēmumus, kas veikti specifikācijas veidošanā
- Ārējam testētājam nav spiediena melot

### Mīnusi
- izstrādātājam kļūst pofig par kvalitāti, jo "QA ar to tiks galā"
- izolācija pasliktina saziņu starp testētājiem un izstrādātājiem
- kļūst par bottleneck, ja ir maz resursu
- neatkarīgiem testētājiem ir mazāk pieredzes ar testējamo objektu līdz ar to tiem var trūkt svarīgas informācijas.

## Testēšanas vadītāja un testētāja uzdevumi

Testēšanas pārvaldību var veikt testēšanas vadītājs, projekta vadītājs, izstrādes vadītājs vai QA vadītājs

Testēšanas vadītājs uzņemas atbildību par testēšanas procesu un veiksmīgu procesu vadību.

Testētājs strādā ar testu sagatavošanu un izpildi, mazāk ar organizatoriska tipa uzdevumiem

### Testēšanas vadītāja uzdevumi

- Organizācijas testēšanas politikas un stratēģijas izstrāde un pārskatīšana
- Plānot testēšanas aktivitātes, izprast testēšanas mērķus un riskus.
- Plānot tehniku izvēli, laika novērtēšanu, resursu izdali, testēšanas līmeņu noteikšana, defektu pārvaldības plānošana
- Testēšanas plāna(u) izstrāde, atjaunošana, koordinēšana ar projekta vadītāju/produkta īpašnieku
- Iniciēt testu [[Testēšanas process#Analīze|analīzi]], [[Testēšanas process#Projektēšana|projektēšanu]], [[Testēšanas process#Izstrāde|izstrādi]], [[Testēšanas process#Izpilde|izpildi]]
- Uzraudzīt testēšanas progresu un rezultātus, veicina testu pabeigšanas aktivitātes.
- Sagatavot testēšanas progresa un kopsavilkuma atskaites
- Pielāgot plānošanas aktivitātes balstoties uz testēšanas rezultātiem, progresu
- Sniegt atbalstu defektu pārvaldības sistēmas uzstādīšanā, testa programmatūras konfigurācijas pārvaldībā
- Ieviest testēšanas progresa un kvalitātes rādītājus 
- Sniegt atbalstu testēšanas atbalsta rīku izstrādē/izvēlē
- Pieņem lēmumus par nepieciešamajām testa vidēm
- Pārstāv un aizstāv testētājus organizācijā
- Izstrādā testētāju karjeras un zināšanu izaugsmes ceļa karti jeb izdomā kā testētājiem kļūt kvalificētākiem.

### Testētāja uzdevumi
- Apskata, ievēro un veicina testēšanas uzdevumu izpildi atbilstoši testēšanas plānam
- Analizē, pārskata un novērtē testa bāzes detaļas
- Identificē un dokumentē testu nosacījumus, veido trasējamību starp testu gadījumiem, testu nosacījumiem un testu bāzi.
- Projektē, izveido un pārbauda testa vides
- Projektē un izstrādā [[Definīcijas#Testa gadījums (Test case)|testa gadījumus]] un testu procedūras
- Sagatavo testa datus
- Sagatavo detalizētu testu izpildes grafiku
- Izpilda testus, novērtē un dokumentē rezultātus
- Lieto piemērotus rīkus testēšanas procesa atvieglošanai
- Automatizē testus
- Novērtē nefunkcionālās īpašības
- Pārskata citu izstrādātos testu gadījumus

# Testu plānošana un novērtēšana

## Testēšanas plāna mērķis un saturs
- Apraksta testēšanas aktivitātes izstrādē un uzturēšanā
- Plānošanu nosaka:
	- organizācijas politika, stratēģija
	- lietotās metodes
	- testēšanas tvērums
	- mērķi 
	- riski
	- ierobežojumi
	- kritiskums
	- testējamība
	- resursu pieejamība
- Testēšanas plānošana ir nepārtraukta visā programmatūras dzīves ciklā
- Plānošana var tikt dokumentēta galvenajā testēšanas plānā un atsevišķos testēšanas plānos sadalījumā pēc līmeņiem vai veidiem

## Aktivitātes
- Tvēruma, mērķu, risku novērtēšana
- Kopējās testēšanas pieejas stratēģijas noteikšana
- Ko testēt?
- Nepieciešamo cilvēku un resursu iesaiste
- Kā tiks veiktas testēšanas darbības?
- Laika rāmja plānošana [[Testēšanas process#Aktivitātes|testēšanas procesa aktivitātēm]]
- Metriku izvēle testēšanas uzraudzībai un kontrolei
- Testēšanas aktivitāšu budžeta plānošana
- Dokumentācijas, tās detalizācijas un struktūras noteikšana

_Tas viss ir tikai ieteikumi, kkas no šī var nebūt vai kkas var nākt klāt_ :DD


## Atgādinājums par IEEE 829

![[Testēšanas plāns#IEEE 829]]


## Testēšanas stratēģija un pieeja

Tipiskās stratēģijas:
- Analītiskā - balstīta uz faktoru analīzi
- Modeļu balstīta - balstīta uz esošu modeli vai nefunkcionālām īpašībām
- Metodiskā - Sistemātiska testu, to nosacījumu izveidi un izpildi katru reizi, kad tiek pievienots jauns vienums
- Procesam vai standartam atbilstoša - vnk seko standartam
- Virzīta vai konsultatīva - seko ekspertu un ieinteresēto personu vadlīnijām
- Regresijas izvairīga - Koncentrējas uz regresijas risku un kā to samazināt. Samazināt potenciālās atkāpes progresā
- Reaģējošā - testētāji reaģē uz testējamo komponentu vai sistēmu notikumiem, kas notiek testu izpildes laikā. Testi tiek projektēti un izstrādāti un var tikt nekavējoties izpildīti balstoties uz zināšanām, kas iegūtas no iepriekšējiem testa rezultātiem (pētnieciskā testēšanas tehnika)

Projektos kombinē šīs stratēģijas atkarībā no projekta prasībām un vajadzībām.
Stratēģijas nosaka [[Statiskā testēšana#Apskates tehnikas|statiskās]] un [[Dinamiskā testēšana#Testēšanas tehnikas|dinamiskās]] tehnikas, līmeņu, tipu izvēli, uzsākšanas un pabeigšanas kritērijus.

## Testu uzsākšanas un pabeigšanas kritēriji
### Uzsākšanas kritēriji
- Prasību, lietotāju stāstu un/vai modeļu pieejamība
- Testējamo vienumu pieejamība
- Nepieciešamo testēšamas rīku pieejamība
- Nepieciešamo testa datu un citu resursu pieejamība

### Pabeigšanas kritēriji
- Plānotie testi ir izpildīti
- Definētais testu pārklājuma līmenis ir sasniegts
- Nenovērsto defektu skaits ir pieļaujamā intervālā
- Paredzamais atlikušo defektu skaits ir pieļaujamā intervālā
- Novērtētās nefunkcionālās īpašības ir pieņemamas (veiktspēja, drošība, lietojamība)
- Zems atlikušais risks (neizpildītie testi, nenovērstie defekti u.c.)
- Sasniegti finansiālie un laika ierobežojami (no monies or due date has come)


## Testu izpildes grafiks

Jāņem vērā testu prioritātes, atkarības, apstiprinājuma testi, regresie testi un efektīvākā testu izpildes secība

Testu prioritāšu noteikšanas kritēriji:
- Kritiska funkcionalitāte
- Kļūdas varbūtība
- Lietošanas biežums
- Kļūdas redzamība gala lietotājam
- Prasību prioritātes
- Kvalitātes īpašības
- Komponentes, kurās kļūdas var novest pie smagām sekām
- Komponenšu sarežģītība
- Projekta riski

**Platuma** testēšana: visus testus izpilda vienlaikus bez secības
**Dziļuma** testēšana: balstās uz prioritāti, vispirms izpilda augstas prioritātes testus

## Faktori, kas ietekmē testēšanas darbu apjomu
Novērtējot testēšanas darbu, tam ieskaita arī to, kas nepieciešams projekta testēšanas mērķu sasniegšanai

Produkta īpašības:
- Saistītie riski
- [[Definīcijas#Testu bāze|Testu bāzes]] kvalitāte
- Produkta izmērs
- Produkta domēna sarežģītība
- Kvalitātes raksturlielumu prasības (drošība, veiktspēja utt.)
- Testēšanas dokumentācijas detalizācijas līmenis
- Prasības likumdošanas un regulatoru atbilstībai

Izstrādes procesa īpašības:
- Organizācijas stabilitāte
- Izmantotais modelis
- Testēšanas pieeja
- Izmantotie rīki
- Testēšanas process
- Laika spiediens

Cilvēku īpašības:
- Iesaistīto cilvēku prasmes un pieredze
- Komandas saliedētība un līderība

Testēšanas reziltāts:
- Atrasto defektu skaits un ietekme
- Nepieciešamais pārstrādāšanas apjoms (cik daudz jāpārtaisa)

## Testēšanas novērtēšanas tehnikas
### Metriku balstīta tehnika
- Lieto līdzīgu projektu metrikas vai tipiskās metriku vērtības (vadās pēc citu projektu datiem)
- Burndown diagrammas (salīdzina padarīto ar neizdarīto)
- Defektu samazināšanas modeļi (cik vēl defekti un to novēršanas laiks)

### Ekspertu balstīta tehnika
- Balstās uz Ekspertiem lai noteiktu, ko un cik daudz testēt
- Plānošanas pokers (min cik vēl jādara pēc pieredzes)
- Wideband Delphi (eksperti min cik vēl jādara pēc pieredzes)

# Testu uzraudzība un kontrole
Skatīt arī [[Testēšanas process#Uzraudzība un kontrole]]

Uzraudzības mērķis: nodrošināt atgriezenisko saiti par testēšanas aktivitātēm.

Uzraudzības informāciju apkopo manuāli un/vai automātiski. To lieto progresa vai pabeigšanas kritēriju novērtēšanai.

Testu kontrole apraksta ko darīt atkarībā no ziņotās informācijas vai metrikām.

Kontroles piemēri:
- Testu prioritāšu maiņa identificēta riska gadījumā
- Testēšanas grafika maiņa resursu nepieejamības dēļ
- Atkārtota testējamā vienuma novērtēšana, vai tas atbilst uzsākšanas vai pabeigšanas kritērijiem

## Metriku nozīme

Metrikas palīdz novērtēt:
- progresu pret plānoto grafiku un budžetu
- Testējamā objekta kvalitāti
- Testēšanas pieejas atbilstību
- Testēšanas aktivitāšu efektivitāti attiecībā pret mērķiem

## Metriku piemēri

- Cik testi tikuši izstrādāti no paredzētajiem
- Paveikto darbu procents
- Testu gadījumu izpilde (izpildīti/neizpildīti, veiksmīgi/neveiksmīgi)
- Defektu informācija (blīvums, atrastie, labotie, atteices reitings, apstiprinājuma testu rezultāti)
- Testu pārklājums
- Uzdevumu pabeigšana resursu piešķiršana un izmantošana
- Testēšanas izmaksas

## Testēšanas ziņojumi

Mērķis: apkopot un komunicēt informāciju par testēšanas darbībām gan testēšanas laikā, gan beigās.

Testēšanas progresa ziņojums satur:
- Testēšanas aktivitāšu statuss
- Progress attiecībā pret testēšanas plānu
- Faktori kas kavē progresu
- Plānotās testēšanas aktivitātes nākamajam periodam
- Testējamā objekta kvalitāte

Testēšanas kopsavilkuma ziņojums satur:
- Testēšanas kopsavilkums
- Informācija par atgadījumiem
- Aktivitāšu novirzes no plāna
- Testēšanas statuss un produkta kvalitāte
- Faktori, kas bloķējuši progresu
- Defekt, testu gadījumu testu pārklājumu, aktivitāšu progress un resursu patēriņa metrikas
- Atlikušie riski
- Atkārtoti lietojamie testēšanas darba produkti

Ziņojumu reālais saturs atšķiras no dzīves cikla, organizācijas, projekta
Testa ziņojumus jāpielāgo adresātam: izstrādātājiem defekti, vadībai progress

# Konfigurācijas pārvaldība

Mērķis: Projekta dzīves cikla laikā izveidot un uzturēt sistēmas, komponentu, testprogrammatūras un to saišu integritāti

![[Pasted image 20240421183431.png]]

Konfigurācijas pārvaldība nodrošina:
- Visiem testējamiem vienumiem ir unikāli id, versiju kontrole, var izsekot veiktajām izmaiņām, ir savstarpējas saites un saites ar testējamo vienumu versijām
- Dokumentācijā atsauces uz identificētiem dokumentiem un programmatūras vienumiem ir nepārprotamas

Konfigurācijas pārvaldības procedūras un rīkus identificē [[Testēšanas process#Plānošana|plānošanas]] laikā

# Riski un testēšana

Skatīt [[Riska pārvaldība]]

Riski iedalās pēc **Iespējamības** un **Ietekmes**

Iespējamība:
- Augsta
- Vidēja
- Zema

Ietekme:
- Kritiska
- Vidēja
- Nenozīmīga

## Produkta un projekta riski

**Produkta risks**: Iespējamība ka darba produkts neatbilst ieinteresēto personu prasībām.

Piemēri:
- Programmatūra neatbilst specifikācijai
- Programmatūra neatbilst ieinteresēto personu vēlmēm
- Sistēmas arhitektūra neatbalsta funkcionālās prasības
- Konkrēts aprēķins ir nepareizs
- Cikla kontroles struktūra programmēta nepareizi
- Sistēmas atbildes laiks nepietiekams pie slodzes
- Gala lietotāja atsauksmes var neatbilst produkta prasībām

**Projekta risks**: Negatīvi ietekmē projekta spēju sasniegt tā mērķus

Piemēri:
- Projekta problēmas:
	- Piegādes, uzdevumu izpildes, pabeigšanas kritēriju izpildes kavēšanās
	- Neprecīzi novērtējumi, līdzekļu pārdale, finansējuma trūkums
	- Novēlotas izmaiņas pieprasa pārstrādi
- Organizatoriskās problēmas
	- Nepietiekamas personāla prasmes
	- Personāla problēmas
	- Lietotāji, personāls nepieejams
- Politiskās problēmas
	- Testētāji nekomunicē savas vajadzības un/vai testēšanas rezultātus
	- Izstrādātāji/testētāji ignorē apskates
	- Var būt nepareiza attieksme pret testēšanu
- Tehniskās problēmas
	- Prasības nav pietiekami labi definētas
	- Ņemot vērā ierobežojumus, prasības var netikt izpildītas
	- Testa vide var nebūt gatava laikā
	- Datu konvertēšana
	- Migrācijas plānošana var kavēties
	- Izstrādes nepilnības var ietekmēt darba produktu
	- Slikta defektu pārvaldība var izraisīt defektu uzkrāšanos un tehnisko parādu
- Piegādātāja problēmas
	- Trešā puse nepiegādā produktu vai bankrotē
	- Līguma problēmas rada sarežģījumus projekta izpildei

## Risku balstīta testēšana

Proaktīvas darbības produkta riska mazināšanai:
- Analīze: riska identificēšana, iespējamības un ietekmes novērtēšana
- Testu plānošana, projektēšana, sagatavošana, izpilde, uzraudzība un kontrole ([[Testēšanas process#Aktivitātes|testēšanas aktivitātes]])

Agrīna risku analīze veicina projekta panākumus

Risku balstītā pieejā riska analīzes rezultātus izmanto, lai noteiktu:
- Pielietojamās testēšanas tehnikas
- Pielietojamos testēšanas līmeņus un tipus (piemēram drošības testēšana, pieejamības testēšana)
- Testējamo apjomu (tvērumu/*scope*)
- Testu prioritātes, atrodot kritiskos defektus
- Papildus aktivitātes riska mazināšanai (piemēram, apmācības)

Lai mazinātu produkta [[Definīcijas#Kļūme (Failure)|kļūmes/atteices]] iestāšanās iespējamību līdz minimumam, jānodrošina disciplinēta pieeja:
- Regulāri analizēt riskus
- Nosakiet kuriem riskiem jāpievērš uzmanība
- Īstenojiet darbības risku mazināšanai
- Izveidojiet [[Riska pārvaldība#Ārkārtas (Contingency) plāns|ārkārtas plānus]], ja iestājas riski