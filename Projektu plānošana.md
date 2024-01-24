# Galvenās tēmas
- [[#Cenošana]]
- [[#Uz plāniem balstīta izstrāde]]
- [[#Laikplānošana]]
- [[#Agile (spējās izstrādes) plānošana]]
- [[#Prognozēšanas paņēmieni]]

> Plānošana ietver darba sadali, problēmu paredzēšana un risinājumu gatavošana (līdzīgi [[Riska pārvaldība|riskiem]], taču šos jāuztver kā lietas kas būs jādara, nevis lietas kas var notikt)

**Projektu plāns** tiek radīts projekta sākumā un skaidro gan komandai, gan klientam kā notiks izstrāde un palīdz izvērtēt progresu.

# Plānošanas secība
## Piedāvājumu rakstīšana (Proposal planning)
> Šajā posmā tiek apskatītas tikai projekta aplēses

Šī posma mērķis ir izvērtēt sistēmas cenu klientiem.

## Sākuma plānošana (Project startup planning)
> Šajā posmā ir zināmas sistēmas prasības, taču nav dizaina vai realizācijas informācijas.

Šajā daļā jānodrošina pietiekami detaļu, lai var veikt izvēles par budžetu un darbaspēku. Tas nodrošina arī uzraudzīšanas mehānismus.

Šī daļa ir obligāta priekš [[#Agile (spējās izstrādes) plānošana|Spējās izstrādes]], lai izvērtētu resursu sadali.

## Izstrādes plānošana (Development planning)

Plānu regulāri jāmaina, jo uzzini vairāk informācijas par projektu un tā izstrādi.

Projekta [[#Laikplānošana|laikplānu]], [[#Cenošana|izmaksu aplēses]] un [[Riska pārvaldība#Risku uzraudzība|riskus]] regulāri jāpārskata.




# Cenošana

## Cena vai izmaksas
**Izmaksas** – naudas daudzums, cik tas izmaksā uzņēmumam.
**Cena** – naudas daudzums, kādu prasa klientam.

> [!warning] Izmaksas gandrīz nekad nesakrīt ar cenu



> [!info] Lai noteiktu izmaksas izstrādātājam, jāveic aplēses (minējumi) (prognozes) (estimations).
> Vērā jāņem šādas izmaksas:
> - aparatūras
> - programmatūras
> - ceļošanas
> - apmācību
> - [[Darbietilpība|darbietilpības]]
> - plašākas organizatoriskās, politiskās, biznesa ietekmes


## Ietekmējošie faktori
| Faktors | Apraksts |
| ---- | ---- |
| Līguma nosacījumi | Klients var piekrist, ka pirmkods paliek izstrādātāja īpašums, kas ļauj to vēlreiz izmantot citur. Tādā gadījumā cena būs mazāka, nekā ja intelektuālais īpašums tiek atdots klientam. |
| Cenas mainība | Ja uzņēmums nav pārliecināts par izmaksām, cena tiks palielināta, lai kompensētu mainīgumu. |
| Finansiālā veselība | Ja uzņēmums ir grūtībās, tas var piedāvāt zemāku cenu, lai uzvarētu konkursu, jo tā ir labāk, nekā to neiegūt. Jebkādi ienākumi ir svarīgāki par peļņu sliktā ekonomikā. |
| Tirgus iespēja | Uzņēmums var samazināt cenu, lai izsistos jaunā tirgū. Ar šādu pamatojumu, uzņēmums var piedāvāt zemas peļņas cenu, kas dod iespēju gūt lielāku peļņu vēlāk un gūt pieredzi. |
| Prasību mainība | Ja ir liela iespēja, ka prasības mainās, cena tiks palielināta, lai kompensētu mainīgajām izmaiņām |

## Cenošanas stratēģijas

### Zemākas cenas noteikšana
- Iespēja izsisties tirgū (Tirgus iespēja)
- Darba spēka saglabāšana (Finansiālā veselība)
### Augstākas cenas noteikšana
- Klients vēlas konstantas cenas līgumu, kas nozīmē, ka cenā jākompensē risku izmaksas.

## Cenošana lai uzvarētu konkursos
- Programmatūru jāceno tā, kā izstrādātājs domā, cik klients ir gatavs maksāt.
- Ja tas ir **mazāk** par izmaksām, jāsamazina funkcionalitāti, lai iekļautos budžetā ar perspektīvu, ka iespējams pievienot funkcionalitāti vēlāk.
- Papildus izmaksas var tikt pievienotas ar prasību izmaiņām un tās var kompensēt oriģināli zemākai cenai.

# Veidot-pirkt lēmumi

Daudzās izstrādes daļās, izstrāde ir lētāka, ja daļu programmatūras iepērk.

Svarīgākie lēmumi, domājot, vai komponenti izstrādāt, vai iepirkt:
- Vai iegādātās programmatūras piegāde būs ātrāka par pašu izstrādātu variantu?
- Vai iepirkuma un tā pielāgošanas izmaksas būs mazākas par pašu izstrādātu programmatūru?
- Vai ārējā atbalsta izmaksas būs mazākas par iekšējo atbalstu (piemēram uzturēšanas izmaksas)?
![[Pasted image 20240108174239.png]]


# Uz plāniem balstīta izstrāde

> [!info] Šis ir "tradicionālais" izstrādes veids lieliem programmatūras projektiem.
> 
> Projekta plāns satur:
> - darāmos darbus
> - kas tos dara
> - laikplānu
> - produktus
> 
> Pārvaldnieki izmanto plānu, lai pamatotu lēmumus un vērtētu progresu
> 

## Plusi
- Organizatoriskās problēmas ir vieglāk ņemamas vērā ar laikplāniem un darbu priekšnosacījumiem **pirms** uzsāk darbu.
## Mīnusi
- Daudzus agrīnos lēmumus jāmaina izstrādes laikā, neparedzētu faktoru dēļ.

## Plānu daļas
- Ievads
- Projekta organizācija
- [[Riska pārvaldība#Risku analīze|Risku analīze]]
- Aparatūras un programmatūras prasības
- Darbu sadalījums
- Projekta laikplāns
- Uzraudzīšanas un [[Ziņošana|ziņošanas]] mehānismi

> [!tldr]+ Papildus projekta plāni
> 
>
| Plāns | Apraksts |
| ---- | ---- |
| [[Konfigurācijas pārvaldība\|Konfigurācijas pārvaldības]] plāns | Apraksta Konfigurācijas pārvaldes procedūras un struktūras |
| Izmantošanas plāns | Paskaidro, kā programmatūru izmantos klienta vidē. Tas iekļauj arī plānu kā migrēt eksistējošo sistēmu datus. |
| Uzturēšanas plāns | Paredz uzturēšanas prasības, izmaksas un [[Darbietilpība\|darbietilpību]]. |
| [[Kvalitātes pārvaldība#Kvalitātes plānošana\|Kvalitātes plāns]] | Apraksta kvalitātes procedūras un standartus, kas tiks izmantoti projektā |
| Validācijas plāns | Apraksta pieeju, resursus un laikplānu kā validēt sistēmu. |

## Plānošanas process

> [!important] Projekta plānošana ir **iteratīvs** process, kurā izmaiņas ir nenovēršamas

![[Pasted image 20240106183351.png]]
[[Projekta plānošanas process.canvas|Projekta plānošanas process (interactive canvas)]]

 > [!tip] Jāveic reālistiskus, nevis optimistiskus pieņēmumus
 
 > [!tip] Vienmēr radīsies ievērojamas problēmas, līdz ar to ierēķini tās laikā.
 
 > [!tip] Iekļauj [[Riska pārvaldība#Ārkārtas Contingency plāns|ārkārtas risinājumus]] plānā, lai novērstu smagus traucējumus laikplānam

> [!tip] Nopietnu problēmu gadījumā jāuzsāk [[Riska pārvaldība#Risku mazināšana (mitigation)|risku mazināšana (mitigation)]]


# Laikplānošana

![[Definīcijas#Laikplānošana (Scheduling)]]


Ir **jāparedz** kalendārais laiks, kuru vajadzēs, lai izpildītu katru darbu, [[Darbietilpība|darbietilpība]], kuru tas prasīs, kā arī kas strādās pie tā.

Jāparedz arī resursi, kā vieta serverī, laiks, kas jāpavada pie specializētas aparatūras (simulatori) un ceļojumu budžets.



## Veicamās darbības
- Sadali projektu darbos, paredzi **laiku** un **resursus**
- Sakārto tos pēc iespējas vienlaicīgi, lai optimāli izmantotu darbaspēku.
- Samazināt darbu atkarības (task dependencies) citam no cita, lai mazinātu kavēšanos, kas radīta no gaidīšanas uz kāda darba paveikšanu.
- Visas darbības ir balstītas uz pārvaldnieka intuīcijas un pieredzes.
![[Pasted image 20240106235735.png]]
[[Laikplāna veidošanas process.canvas|Laikplāna veidošanas process (interactive canvas)]]

## Grūtības
- Ir grūti paredzēt problēmu sarežģītību, līdz ar to arī veidošanas izmaksas
- Produktivitāte nav proporcionāla cilvēku skaitam, kas strādā pie darba
- Pievienot cilvēkus pie projekta, kas kavējas, nepalīdzēs projektam tikt pabeigtam ātrāk jo jaunpienācējus ir jāinformē par projekta progresu un uz ko jākoncentrējas.
- Negaidītais **vienmēr** notiek. Vienmēr atstāj laiku ārkārtas gadījumiem.

## Laikplāna prezentēšana

> [!info] Parasti šim izmanto grafikus
> 
> Parādi projekta iedalījumu darbos. Tiem nevajadzētu būt pārāk maziem. Jātēmē uz 1 vai 2 nedēļām katram darbam.

Uz kalendāriem balstīta prezentācija izmantos stabiņu diagrammas, kas parāda darbības vai resursus pret laiku.

Aktivitāšu (darbu) tīkli parāda darbu priekšnosacījumus.

## Aktivitāte (darbs)

![[Definīcijas#Darbs/Aktivitāte (Activity/Task)]]

Katrai aktivitātei ir:
- laika posms kalendārajās dienās vai mēnešos
- [[Darbietilpība|Darbietilpības]] prognoze, kas parāda [[Definīcijas#Persondiena/Personmēnesis (Person-days/Person-months)|persondienas vai personmēnešus]], cik tie aizņem.
- Termiņš, līdz kuram jābeidz.
- Darba gala punkts (dokuments, pārskata sanāksme, veiksmīga testu izpilde vai kāda cita konkrēta darbība)

## Darbu tīkla piemērs


![[Pasted image 20240107005429.png]]
Šeit redzams kā daļa no darbiem ir savietoti paralēli, lai tos var darīt vienlaicīgi dažādas komandas. ^1bp4xd

## Laikjoslas tabulas - Ganta diagrammas

![[Pasted image 20240107011257.png]]
Apzīmē darbus, kā arī kad un cik ilgi tos jādara. ^3fjkyt


## Tabulēti darbi

![[Pasted image 20240107013019.png]]

## Aktivitāšu stabiņu diagramma 

![[Pasted image 20240107013536.png]]

Šī ir līdzīga [[#Laikjoslas tabulas - Ganta diagrammas|Ganta diagrammai]], taču arī iekļauj [[Definīcijas#Šķirtne (Milestone)|šķirtnes]] un to darbus, kuriem jābūt izpildītiem.

## Darbinieku sadalījuma diagramma

![[Pasted image 20240107014650.png]]

Tās apraksta kuri darbinieki kuros periodos strādā pie konkrētiem darbiem.

# Agile (spējās izstrādes) plānošana

[[Definīcijas#Spējā izstrāde (Agile)|Spējā izstrāde]] ir iteratīva pieeja, kurā izstrādi un piegādi klientiem veic periodiski un pa daļām. Atšķirīgi no [[#Plānošanas process|plānošanas]], šīs daļas tiek noteiktas izstrādes laikā.

> [!hint]
> Tas, kas tiek iekļauts katrā daļā atšķiras no progresa un klienta prioritātēm.
> Prioritātes mainīsies, taču tas neietekmēs plānu, jo spējās izstrādes ietvaros plāns ir ierobežots ar daļu, kas nozīmē, ka nav daudz jākoriģē, lai izmaiņām pielāgotos.

## Spējās izstrādes plānošanas soļi
- Izdevumu(?) plānošana (Release planning), kas ieplāno izdevumus vairākus mēnešus uz priekšu un nosaka, kādai funkcionalitātei jābūt nākamajā sistēmas izdevumā.
- Iterāciju ([[Definīcijas#Spējās izstrādes sprints (Agile sprint)|sprintu]]) plānošanā tiek aplūkots īsāks periods, kurā plāno nākamo sistēmas izdevumu.

## Darbu sadale

Vienam darbam būtu jāaizņem 4-16 stundas.
**Visiem** darbiem jābūt paveiktiem, lai izveidotu iterācijā rindoto funkcionalitāti.
Individuāli izstrādātāji piesakās darbiem, kurus tie veiks.

> [!info] Priekšrocības šai metodei
> - Visa komanda gūst priekšstatu par darāmajiem darbiem.
> - Izstrādātājiem ir īpašuma sajūta, ka tiem pieder tas darbs (skatīt [[Cilvēku pārvaldība|cilvēku vajadzību nodrošināšanu]])

## Programmatūras piegāde

Katras iterācijas beigās programmatūru piegādā klientam.
Ja kāda funkcionalitāte netiek paveikta atvēlētajā laikā, tiek samazināts darba apjoms.

> [!warning] Piegādes laiku nekad nepārceļ

## Spējās plānošanas problēmas

- Spējā plānošana ir ļoti atkarīga no klienta sadarbības un pieejamības.
- Reizēm to var būt grūti organizēt, jo klientam arī ir savas prioritātes, kas tam neļauj iesaistīties plānošanā.
- Reizēm klients var būt pieradis pie tradicionālas plānošanas un atduras pret grūtībām veiksmīgi iesaistīties spējās plānošanas procesā

## Spējās plānošanas pielietojums

- Ļoti labi strādā **mazās, stabilās komandās**, kas labi sadarbojas.
- Lielās un ģeogrāfski attālās grupās vai nestabilās grupās ir **gandrīz neiespējami** panākt visu iesaisti plānošanā, kas vajadzīga spējai projekta pārvaldei.

![[Darbietilpība#Projektu plānošana Agile (spējās izstrādes) plānošana Spējās izstrādes prognozēšana|Spējās izstrādes prognozēšana]]


# Projektu plānošanas darāmie darbi

## Pirmā daļa
- Noteikt projekta apjomu
- Noteikt izpildāmību (feasibility)
- [[Riska pārvaldība#Risku analīze|Risku analīze]]
- Definēt pieejamos resursus
- Noteikt pieejamos cilvēkresursus
- Noteikt vairāklietojamo programmatūru
- Identificēt vides resursus

## Otrā daļa
- Paredzēt [[#Cenošana|cenu]] un [[Darbietilpība|darbietilpību]]
	- "Skaldi un valdi" problēmu
	- Veido 2 vai vairākus minējumus izmantojot apjomu, [[Definīcijas#Funkcionālie punkti (Function points)|funkcionālos punktus]], [[Projektu plānošana#Aktivitāte darbs|darbus]], lietošanas piemērus (use cases)
	- Apvieno minējumus, gūstot kopēju priekšstatu
- Izveido [[#Laikplānošana|laikplānu]]
	- Veido jēdzīgu darbu sarakstu
	- Definē [[Projektu plānošana#^1bp4xd|darbu tīklu]]
	- Izmanto laikplānošanas rīkus lai radītu [[Projektu plānošana#^3fjkyt|laikjoslas tabulu]]
	- Definē laikplāna uzraudzīšanas mehānismus

# Resursu, izmaksu, laikplāna prognozēšana

Resursu, izmaksu[^1] un laikplāna darbiem prognozēšanai vajadzīga:
- pieredze
- pieeja vēsturiskiem datiem un metrikām
- Drosme pieturēties kvantitatīviem datiem, kamēr ir pieejama tikai kvalitatīva informācija.

Prognozēšanai ir risks un šis risks noved pie iespējamībām.


## Kādēļ projekti kavējas?
- **Nereālistiski laika limiti**, kurus dod kāda partija ārpus izstrādes komandas.
- Mainīgas klientu prasības
- Godīgi slikti novērtēts patērējamais laiks uz darbiem, kad sāka projektu.
- Paredzami vai neparedzami [[Riska pārvaldība|riski]].
- Neparedzamas tehniskas problēmas
- Neparedzamas [[Cilvēku pārvaldība|cilvēkresursu]] problēmas
- Komunikācijas problēmas
- Pārvaldība neatzīst, ka kavēšanās notiek, kas nozīmē, ka bezdarbības dēļ projekts iepaliek vēl vairāk.

## Prognožu uzticamība
![[Pasted image 20240107210058.png]]
Prognozes projekta gaitā kļūst uzticamākas, taču svarīgākās prognozes parasti veic projekta sākumā.


## Prognozēšanas paņēmieni

> [!tip] Humoriņi
> [[Humoriņi#Deviņdesmit-deviņdesmit likums (Ninety-ninety rule)|Deviņdesmit-deviņdesmit likums]]
>
> [[Humoriņi#Hofstadtera likums (Hofstadter's law)|Hofstadtera likums]]
>
>[[Humoriņi#Freda Bruksa likums (Fred Brooks' law)|Freda Bruksa likums]]

> [!info]- Gadījumi iz dzīves
> - Neveiksmīgi un veiksmīgi projekti kādā datorizstrādes komercsabiedrībā 90.-to gadu vidū
> - Šveices baznīckungu pasūtījums
> - Kā neizgāzās Valsts ieņēmumu informācijas sistēmas projekts

Divi galvenie prognozēšanas paņēmieni:
- [[#Uz pieredzi balstīti paņēmieni]]
- [[#Algoritmiska izmaksu modelēšana]]

### Uz pieredzi balstīti paņēmieni

Visas prognozes tiek balstītas uz pārvaldnieka pieredzi agrākajos projektos un nozares darbos. Tas nozīmē, ka tā ir pārvaldnieka atbildība veikt informētus minējumus par vajadzīgo [[Darbietilpība|darbietilpību]], izmaksām, resursiem.

### Algoritmiska izmaksu modelēšana

Šādā pieejā, prognozēšanai izmanto formulas izmantojot vienkāršākpieejamas prognozes, kā apjoms, procesu raksturojumi un darbaspēka raksturojums.

## Resursi
Projekta resursi iedalās 3 grupās, kurām ir vairāki parametri, kurus jāņem vērā:
- Cilvēkresursi
	- Ģeogrāfiskā atrašanās vieta
	- Prasmes
	- Cilvēku skaits
- Vides resursi
	- Programmatūras rīki
	- Aparatūra
	- Tīkla resursi
- Vairākkārt lietojamā programmatūra
	- OTS (Off-The-Shelf) komponentes jeb jau gatavās komponentes
	- Full experience komponentes jeb komponentes par kurām ir daudz pieredzes vai jau eksistējošas komponentes, kurām vajadzīga minimāla koriģēšana, lai tās varētu savietot ar projektu.
	- Partial experience komponentes jeb komponentes, kurām vajadzīgi netriviāli pārveidojumi, lai tās savietotu ar projektu.
	- Jaunas komponentes, jeb tās, kuras jāveido "no nulles"

## Darbaspēka prasības

Vajadzīgo darbaspēku nevar aprēķināt dalot paredzēto izpildes laiku ar vajadzīgo izpildes laiku.

Darbinieku skaits mainās atkarībā no izstrādes stadijas.

Jo vairāk cilvēku strādā pie projekta, jo vairāk kopējās darbietilpības nepieciešams.


# Projekta prognozēšana
Lai prognozētu projektu, galvenās detaļas:
- Jāprognozē projekta apjomu
- Skaldīšana (dekompozīcija)
- Vēsturiskās metrikas
- Izmantoti vismaz 2 paņēmieni
- Iespējamības ir nenovēršamas.

## Projekta prognozēšanas paņēmieni

- Agrākā pieredze
- Parastās prognozēšanas metodes
	- Darbu skaldīšana un [[Darbietilpība|darbietilpības]] prognozes
	- Apjoma (piem., Funkcionālie punkti) prognozes
- Empīriskie modeļi
- Automātiskie rīki



[^1]: [[#Cena vai izmaksas|Ir svarīga starpība starp cenu un izmaksām]]