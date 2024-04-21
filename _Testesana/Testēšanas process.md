# Testēšanas process

Testēšanas process ir balstīts uz [ISO/IEC/IEEE 29119-1:2022](https://www.iso.org/standard/81291.html) standartu, taču nav viena tāda universāla testēšanas procesa.
Ir kopīgas aktivitāšu kopas, bez kurām būs mazāka iespēja sasniegt izvirzītos mērķus.

# Testēšanas procesa faktori

- Programmatūras dzīves cikla modelis
- Testēšanas līmeņi, testu veidi
- Biznesa domēns
- Darbību ierobežojumi, to skaitā budžets, resursi, laika grafiks, sarežģītība, līguma, regulatora prasības.
- Organizatoriskā politika, prakse
- Nepieciešamie iekšējie, ārējie standarti.
# Aktivitātes

- Plānošana
- Analīze
- Projektēšana
- Izstrāde
- Izpilde
- Pabeigšana
- Uzraudzība un kontrole

![[Pasted image 20240421103620.png]]
## Plānošana
- Testēšanas mērķu definēšana
- Pieeju definēšana mērķu sasniegšanai
	- Tehnikas izvēle
	- Uzdevumu definēšana
	- Testēšanas laika grafiks
- Var tikt pārskatīts caur atgriezenisko saiti no testu [[#Uzraudzība un kontrole|uzraudzības un kontroles]].

**Rezultāts**: testēšanas plāns(i)

## Analīze
> **Ko testēt?**

Analīze jeb **prasību analīze**
- Nosaka testu bāzi
	- Prasību specifikācijas:
		- Biznesa prasības
		- Funkcionālās prasības
		- Sistēmas prasības
		- Lietotāju stāsti
		- Epiki
		- Lietošanas gadījumi
		- Citi darba produkti, kas norāda vēlamo funkcionālo un nefunkcionālo komponentu vai sistēmas darbību.
	- Projektējuma dokumentācija (arhitektūra, UML, saskarnes)
	- Sistēmas kods, datu bāze, vaicājumi saskarnes
	- [[Riska pārvaldība#Risku analīze|Riska analīzes]] ziņojumi, kuros var ņemt vērā komponenta vai sistēmas funkcionālos, nefunkcionālos, strukturālos aspektus.
- Izvērtējot testa bāzi, identificē iespējamo defektu veidus, piemēram:
	- Prasību neviennozīmīgumu
	- Iztrūkumus
	- Neatbilstības
	- Neprecizitātes
	- Pretrunas
	- Liekus apgalvojumus
- Nosaka testējamās funkcijas un funkciju kopas
- Nosaka testu definēšanas un prioritizēšanas nosacījumus katrai funkcijai, funkciju kopām
- Nodrošina izsekojamību starp katru testa bāzes elementu un noteiktajiem testu nosacījumiem
- Izmērāmu testu pārklājuma kritēriju noteikšana

**Rezultāts**: Prioritizēti testa nosacījumi
## Projektēšana
> **Kā testēt?**

- [[Definīcijas#Testa gadījums (Test case)|Testa gadījumu]], gadījumu kopu projektēšana, to prioritātes
- Nepieciešamo testa datu noteikšana
- Testa vides projektēšana, rīku identificēšana
- Izsekojamība starp testa bāzi, testa nosacījumiem, testa gadījumiem
- [[Definīcijas#Defekts (Defect)|Defektu]] identificēšana testa bāzē.

**Rezultāts**: [[Definīcijas#Testa gadījums (Test case)|Testa gadījumi]] (augsta līmeņa testa gadījumi, testa dati, vides, infrastruktūra, rīki)
## Izstrāde
> **Vai viss gatavs pārbaudei?**

- Izstrādā testu programmatūru
- Izstrādā testu dokumentāciju
- Procedūru izstrāde, prioritāšu noteikšana (automātisko skriptu izstrāde)
- Testu komplektu izveide no testu procedūrām un skriptiem
- Testu komplektu iekļaušana testu izpildes grafikā
- Testa vides, infrastruktūras veidošana
- Testa datu veidošana, to ielādes nodrošināšana
- Izsekojamības pārbaude un atjaunināšana starp testa bāzi, testa nosacījumiem, [[Definīcijas#Testa gadījums (Test case)|testa gadījumiem]], procedūrām, komplektiem

**Rezultāts**:Testa komplekti, testu izpildes grafiks, automatizēti testa skripti, virtualizācija.
## Izpilde
- Izpilde saskaņā ar grafiku
- Testējamo objektu versiju žurnalēšana
- Izpilda testus manuāli vai ar rīkiem
- Salīdzina faktiskos ar gaidāmajiem rezultātiem
- Rezultātu analīze, lai noteiktu to iespējamos cēloņus
- [[Definīcijas#Defekts (Defect)|Defektu]] ziņošana, pamatojoties uz novērotajām [[Definīcijas#Kļūme (Failure)|kļūmēm]]
- Testa izpildes rezultāta žurnalēšana
- Testu izpildes atkārtošana pēc kļūdu novēršanas (labota kļūda, tests, regresijas pārbaude)
- Izsekojamības pārbaude un atjaunināšana starp testa bāzi, testa apstākļiem, [[Definīcijas#Testa gadījums (Test case)|testa gadījumiem]], testa procedūrām, testa rezultātiem.

**Rezultāti**: Statusu dokumentācija, ziņojumi par defektiem, dokumentācija par testu, rīkiem, testprogrammatūru

## Pabeigšana

- Pārbauda, vai visi [[Definīcijas#Defekts (Defect)|defektu]] ziņojumi ir aizvērti.
- Reģistrē izmaiņu pieprasījumus par neatrisinātajiem defektiem
- Kopsavilkuma izveide, tā komunicēšana ieinteresētajām personām
- Testa vides, datu, infrastruktūras , testēšanas programmatūras arhivēšana atkārtotai izmantošanai
- Testa programmatūras nodošana uzturēšanas komandām, citām komandām un personām
- Analizē gūto pieredzi, lai noteiktu vajadzīgās izmaiņas turpmākajām iterācijām, projektiem
- Izmanto informāciju, lai uzlabotu testēšanas procesa biedrumu/gatavību

**Rezultāts**: Kopsavilkuma ziņojumi, pabeigta testprogrammatūra, izmaiņu pieprasījumi, testēšanas procesa pilnveidošanas ieteikumi par nākamjiem projektiem
## Uzraudzība un kontrole
- Nepārtraukts process visā izstrādes gaitā
- Novērtē progresu pret plānoto
- Novērtē progresu mērķu sasniegšanai
- Testu izpildes kritēriju *(exit criteria)* novērtējums.
	- Pārbauda rezultātus un žurnālfailus ar noteiktiem pārklājuma kritērijiem
	- Komponentu vai sistēmas kvalitātes līmeņa novērtēšana, pamatojoties uz testu rezultātiem un žurnālfailiem
	- Nosaka vai nepieciešami papildus testi
- Komunicē progresu ar iesaistītām personām.

**Rezultāts**: testu atskaites, tai skaitā progresa atskaites

Skatīt arī [[Testēšanas pārvaldība#Testu uzraudzība un kontrole]]


## Izsekojamība
Svarīgi ir nodrošināt izsekojamību visiem testēšanas darba produktiem ar testu bāzi

>[!info]
>Kvalifikācijas darbā ir jānodrošina vienībtestu un prasību izsekojamība

