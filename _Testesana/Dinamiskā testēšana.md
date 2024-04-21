# Definīcija
![[Definīcijas#Dinamiskā testēšana (Dynamic testing)|D]]

# Testēšanas tehnikas izvēles faktori
- Sistēmas sarežģītība
- Regulējošie standarti
- Klienta vai līguma prasības
- Riska līmeņi un tipi
- Pieejamā dokumentācija
- Testētāju zināšanas un prasmes
- Pieejamie rīki
- Laiks un budžets
- Programmatūras izstrādes dzīves cikla modelis
- Sistēmā sagaidāmo defektu tipi

# Testēšanas tehniku kategorijas
- [[Definīcijas#Melnās kastes testēšana (Black-box testing)|Melnās kastes testēšana]]
- [[Definīcijas#Baltās kastes testēšana (White-box tests)|Baltās kastes testēšana]]
- Pieredzes balstītas testēšanas tehnikas

# Melnās kastes testēšana

![[Definīcijas#Melnās kastes testēšana (Black-box testing)|]]

Piemērota **augsta** līmeņa testiem.

Testa nosacījumi, testa gadījumi un testa dati tiek iegūti no testu bāzes (programmatūras prasības, specifikācijas, lietošanas gadījumi, lietotāju stāsti)

- Piemēro gan funkcionālai, gan nefunkcionālai testēšanai.
- Pieņem ka prasības ir pilnīgas un nosedz lietotāju vēlmes
- Neredz funkcionalitāti, kas nav iekļautas prasību dokumentācijā
- Sistēmas darbība nav zināma
- Paredz testējamā objekta ievades un izvades, nepārzinot iekšējo struktūru
- Pārklājumu mēra balstoties uz testu bāzes vienumiem un testēšanas tehniku

## Melnās kastes testēšanas tehnikas

- Sadalīšana ekvivalences klasēs
- Robežvērtību analīze: 
- Lēmumu tabulas
- Stāvokļu pārejas testēšana
- Lietošanas gadījuma testēšana

### Ekvivalences klases

Ievadi dala klasēs

### Robežvērtību analīze

Ekvivalences klašu tehnika, taču uzlabo nosakot robežas, pie kurām ievērojami mainās izvade.

### Lēmumu tabulas

Izolē konkrētus nosacījumus un testē katru šo nosacījumu kombināciju.
Tipiski nosacījumi ir būla vērtības *(true/false)*

### Stāvokļu pārejas testēšana

Atrod visus stāvokļus, testē pārejas caur visiem iespējamiem stāvokļu ceļiem.
![[Pasted image 20240420230502.png]]

### Lietošanas gadījuma testēšana

Apskata veidus kā lietotājs testējamo objektu izmantos.

# Baltās kastes testēšana
![[Definīcijas#Baltās kastes testēšana (White-box tests)|D]]
Balstīta uz testējamā objekta iekšām: kodu, arhitektūru utt.

Piemērota **zema** līmeņa testiem

## Testēšanas tehnikas

- Komandu *(statement)* testēšana un pārklājums
- Lēmumu/zaru testēšana un pārklājums
- Nosacījumu testēšana
- Daudznosacījumu testēšana

Mērķis: Testa pārklājumu mērīšana un Strukturālo testa gadījumu projektēšana


### Komandu testēšana
Panāk, ka tiek noklāti visi komandu izsaukumi

### Lēmumu/zaru testēšana
Panāk ka noklātas visas šķautnes.

### Nosacījumu testēšana
No pirmkoda atrod visas predikātu kombinācijas un testē visas predikātu kombinācijas, pielāgojot ieejas datus predikātiem.
![[Pasted image 20240420231838.png]]

# Pieredzes balstītas testēšanas tehnika

Testētājs pārzin biznesa domēnu, programmatūru, lietotāja intereses u.c., kas tam ļauj ātri atrast lielākās kļūmes, kā arī potenciālās problēmas un to ietekmi.

Nav strukturēta un pārklājumu nevar mērīt, bet lēta un piemērota ja nav dokumentācijas.
![[Pasted image 20240420232606.png]]
Tehnikas:
- Kļūdu minēšana
- Pētnieciskā testēšana
- Kontrolsarakstu testēšana

## Kļūdu minēšana

Testētājs uzmin, kur varētu parādīties kļūdas, taču labi jāpārzin programmatūra.

## Pētnieciskā testēšana

Testus rada dinamiski, balstoties uz iepriekšējo testu rezultātiem.
Problemātiskiem moduļiem dabiski radīsies vairāk testu.

>[!info]
>Pētnieciskā testēšana =/= Ad hoc
>Ad hoc attiecas uz kaut ko neplānotu, lai atrastu kļūdu, tā ir nestrukturēta.
>Pētnieciskā testēšana attīstās dinamiski, balstoties uz iepriekšējo gadījumu izpildi

## Kontrolsarakstu testēšana

Testus strukturē, lai apstvertu kontrolsarakstu nosacījumus.

Var veidot jaunus kontrolsarakstus vai papildināt esošos.

Viegli, ātri, bet var radīt caurumus pārklājumos un sarežģītas sistēmas ir grūti aprakstīt ar kontrolsarakstiem.

# Kopsavilkums

Ir daudz dinamiskās testēšanas tehniku, vislabāk tās ir kombinēt.
Testu kvalitāte ir ļooti atkarīga no testētāja spējām, pieredzes, intuīcijas.


