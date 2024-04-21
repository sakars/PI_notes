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
- Testu bāzes kvalitāte
- 


