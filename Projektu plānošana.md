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

> [!info] Lai noteiktu izmaksas izstrādātājam, jāveic aplēses.
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
| [[Konfigurācijas pārvalde\|Konfigurācijas pārvaldes]] plāns | Apraksta Konfigurācijas pārvaldes procedūras un struktūras |
| Izmantošanas plāns | Paskaidro, kā programmatūru izmantos klienta vidē. Tas iekļauj arī plānu kā migrēt eksistējošo sistēmu datus. |
| Uzturēšanas plāns | Paredz uzturēšanas prasības, izmaksas un [[Darbietilpība\|darbietilpību]]. |
| [[Kvalitātes plānošana\|Kvalitātes plāns]] | Apraksta kvalitātes procedūras un standartus, kas tiks izmantoti projektā |
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
# Agile (spējās izstrādes) plānošana

# Prognozēšanas paņēmieni

