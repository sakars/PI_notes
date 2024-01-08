![[Definīcijas#Darbietilpība (Effort)]]


# Prognozēšana

## Agrākā pieredze

Ar agrāko pieredzi ir iespējams prognozēt darbietilpību. Šis nav uzticams veids un ir ļoti atkarīgs no pārvaldnieka pieredzes.

Parasti nosaka [[Definīcijas#Nodevumi (Deliverables)|nodevumus]] un saliek izklājlapā. Tos prognozē individuāli un aprēķina kopējo darbietilpību.

Parasti noder šo darīt grupā, katram grupas biedram paskaidrojot savu prognozi.

> [!danger] Problēmas
> - Ir grūti prognozēt projektus, kuriem nav daudz kopīga ar iepriekšējiem projektiem.
> - Programmatūra strauji attīstās, kas nozīmē, ka projekts lietos jaunas, vēl neizpētītas tehnoloģijas.
> - Ja neesi strādājis ar šīm tehnoloģijām, iepriekšēja pieredze nedos precīzas prognozes.




## Darbu skaldīšana un darbietilpības prognozes

Darbu skaldīšana padara prognozes uzticamākas, jo maziem darbiem prognozes kļūda ir mazāka.

## Apjoma prognozes

Apjoma prognozes ietver projekta izvērtēšanu Funkcijas punktu vai pēc kāda cita parametra un darbietilpību prognozē pēc tā.

## Empīriskie modeļi

Empīriskie modeļi paredz darbietilpību, salīdzinot to ar agrāko projektu apjomu un darbietilpību.

> [!info] Galvenā formula
> $$E=a \cdot S^{b}$$
> $E$ – Darbietilpība (Effort)
> $S$ – Apjoms, parasti mēra koda rindās, bet var būt izteikts arī funkcionālajos punktos.
> $a$ – konstante vai darināts mainīgais, kas atkarīgs no projekta sarežģītības
> $b$ – empīriski noteikta eksponente

### COCOMO

![[Definīcijas#COCOMO]]

Vienkāršais COCOMO

$$ \text{Darbietilpība}=a \cdot (\text{KLOC})^b$$
$$\text{Laiks}=a \cdot (\text{Darbietilpība})^d$$
$$\text{Vajadzīgais cilvēku skaits}=\frac{\text{Darbietilpība}}{\text{Laiks}}$$
KLOC - [[Definīcijas#Pirmkoda rindas (Lines Of Code) (LOC)|Kilorindas koda]].

| Projekta veids | a | b | c | d |
| ---- | ---- | ---- | ---- | ---- |
| Organisks | 2.4 | 1.05 | 2.5 | 0.38 |
| Daļēji atdalīts (Semi-Detached) | 3.0 | 1.12 | 2.5 | 0.35 |
| Iegults | 3.6 | 1.20 | 2.5 | 0.32 |

**Organisks** – Komanda ir adekvāti maza un problēma ir labi saprotama, tikusi atrisināta agrāk un komandai ir izpratne par problēmu.

**Daļēji atdalīts** – projekta izmērs, komandas pieredze, zināšanas par problēmām ir starp Organisku un Iegultu. Tiem vajag papildus laiku, tie ir ne-triviāli, tiem vajag radošumu. Kā piemērs ir kompilatori un iegultās sistēmas.

**Iegults** – sarežģīts projekts, par kuru komandai ir maz zināšanu, tam vajag lielu radošumu. Šādai programmatūrai vajag lielu komandas izmēru, izstrādātājiem jābūt pieredzējušiem un radošiem, lai veidotu šāda līmeņa projektus.

### COCOMO II

COCOMO II ir prognozēšanas modeļu hierarhija. Tas ir daudz nobriedušāks modelis nekā COCOMO

- **Lietotņu kompozīcijas modelis** – tiek izmantots agrīnajos posmos, kad prototipē lietotāja saskarnes, plāno programmatūru, apskata jaudu, sistēmu mijiedarbību un tehnoloģijas briedumu.
- **Agrīnā dizaina posma modelis** – lietots, kad prasības ir nostabilizētas un pamata projekta arhitektūra ir nodibināta.
- **Pēc arhitektūras posma modelis** – lietots programmatūras izstrādes laikā
### Citi modeļi

$\text{Darbietilpība} = 5.2 \cdot (\text{KLOC})^{0.91}$ – Walstona-Fēliksa (Walston-Felix) modelis

$\text{Darbietilpība}=5.5+0.73 \cdot (\text{KLOC})^{1.16}$ – Beilija-Basili (Bailey-Basili) modelis

$\text{Darbietilpība}=5.288 \cdot (\text{KLOC})^{1.047}$ – Doty modelis, ja $\text{KLOC}>9$

### Funkcionālie punkti (Function points (Albrecht))

![[Definīcijas#Funkcionālie punkti (Function points)]]

| Informācijas domēni | Skaits |  | Vienkāršais<br>reizinātājs | Vidējais<br>reizinātājs | Sarežģītais<br>reizinātājs |  | Kopā |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| Ārējās ievades (EIs) |  | X | 3 | 4 | 6 | = |  |
| Ārējās izvades (EOs) |  | X | 4 | 5 | 7 | = |  |
| Ārējie vaicājumi (EQs) |  | X | 3 | 4 | 6 | = |  |
| Iekšējās loģiskās datnes (ILFs) |  | X | 7 | 10 | 15 | = |  |
| Ārējās saskarnes datnes (EIFs) |  | X | 5 | 7 | 10 | = |  |
| Summa |  |  |  |  |  |  |  |

$$\text{FP}=\text{Kopsumma} \cdot \left(0.65 + 0.01 \cdot \sum{(Fi)} \right)$$
$Fi \ (i = 1 \text{ to } 14)$  – vērtības koriģēšanas faktori, kas ir balstīti uz atbildēm jautājumiem
1. Vai sistēmai vajadzīga uzticama rezervju sistēma un atgūšana?
2. Vai lietotnei vajadzīga īpaša datu pārnese?
3. Vai ir izkliedēta apstrāde?
4. Vai vajadzīga jauda?
5. Vai sistēma darbosies eksistējošā, smagi izmantotā vidē?
6. Vai sistēmai vajadzīga tiešsaistes datu ievade?
7. Vai tiešsaistes datu ievadei vajadzīgi vairāki logi vai darbības?
8. Vai iekšējās loģiskās datnes tiek atjaunotas tiešsaistē?
9. Vai ievades, izvades, datnes, vaicājumi ir sarežģīti?
10. Vai iekšējā apstrāde ir sarežģīta?
11. Vai kodu jāveido vairākkārt izmantojamu?
12. Vai pārveidojums un instalēšana ir iekļauta dizainā?
13. Vai sistēma ir izveidota priekš vairākām instalācijām dažādās organizācijās?
14. Vai lietotne ir dizainēta, lai nodrošinātu izmaiņas un lietojamību lietotājam?
Katru jautājumu jāatbild skalā 0 (nav piemērojams/svarīgs) - 5 (pilnībā nepieciešams)

Konstantās vērtības un reizinātāji ir noteikti empīriski.

#### Piemērs
![[Pasted image 20240108123846.png]]

Pieņemot visus $Fi=5$:

$$\text{FP}=82 \cdot \left(0.65 + 0.01 \cdot 70 \right)=82 \cdot 1.35 = 110.7$$

#### Funkcijas punktu modeļi

Daži no FP modeļiem:
- $\text{Darbietilpība}=-91.4+0.355 \cdot \text{FP}$ Albrehta un Gafneja (Albrecht and Gaffney) modelis
- $\text{Darbietilpība}=-37+0.96 \cdot \text{FP}$ – Kemerera (Kemerer) modelis
- $\text{Darbietilpība}=-12.88 + 0.405 \cdot \text{FP}$ – Maza projekta regresijas modelis

![[Pasted image 20240108125017.png]]
[QSM](https://qsm.com) Vidējais pirmkoda rindu daudzums uz vienu funkcionālo punktu pēc valodas.


## Uz procesiem balstīta prognozēšana

No "procesu ietvara" iegūst ietvara aktivitātes.

Piemēri ietvara aktivitātēm:
- Komunikācija
- Veidošana
- Plānošana
- Izlaišana
- Modelēšana

![[Pasted image 20240108132400.png]]
Piemērs aprēķiniem

### Prognozēšana ar Izmantošanas veidiem (use-cases)

$$\text{LOCestimate}=N \cdot \text{LOCavg}+\left[ \left( \frac{\text{Sa}}{\text{Sh}} -1 \right) + \left( \frac{\text{Pa}}{\text{Ph}} - 1 \right) \right] \cdot \text{LOCadjust}$$

$\text{LOCestimate}$ – koda rindu prognoze
$N$ – izmantošanas veidu skaits 
$\text{LOCavg}$ – vēsturiskais vidējais koda rindu skaits katram izmantošanas veidam
$\text{LOCadjust}$ – atspoguļo labojumu, kas balstīts uz $n$ procentiem no $\text{LOCavg}$, kur $n$ ir starpība starp šo projektu un "vidējiem" projektiem.

$\text{Sa}$ – scenāriju skaits uz izmantošanas veidu
$\text{Sh}$ – vidējais scenāriju skaits uz izmantošanas veidu uz šāda veida apakšsistēmu
$\text{Pa}$ – lapu skaits uz izmantošanas veidu
$\text{Ph}$ – vidējais šāda veida apakšsistēmas lapu skaits uz izmantošanas veidu

#### Piemērs
![[Pasted image 20240108133913.png]]

## Objektu orientēta prognozēšana

Objektu orientēta prognozēšana dala darbu objektos. Izmantojot prasības, modelē objektus, veido izmantošanas gadījumus. No analīzes modeļa nosaka galveno klašu skaitu. Kategorizē saskarnes veidus lietotnei un izveido reizinātāju atbalsta klasēm.

| Saskarnes veids | Reizinātājs |
| ---- | ---- |
| Bez grafiskās saskarnes | 2.0 |
| Tekstveida saskarne | 2.25 |
| Grafiskā saskarne | 2.5 |
| Sarežģīta grafiskā saskarne | 3.0 |

Reizina galveno klašu skaitu ar reizinātāju, lai noteiktu atbalsta klašu skaitu. Kopējo klašu skaitu (galvenās + atbalsta) sareizina ar vidējo vajadzīgo darba vienību skaitu klasei. Lorenz un Kidd iesaka 15-20 persondienu uz klasi.

Salīdzina klašu prognozi, reizinot vidējo darba vienību skaitu uz lietošanas veidu.

## [[Projektu plānošana#Agile (spējās izstrādes) plānošana|Spējās izstrādes]] prognozēšana
 
Katru lietotāja gadījumu (user scenario) jāvērtē atsevišķi prognozēšanai.

Gadījumu sadala izstrādes darbu kopā, kurus vajadzēs, lai to izstrādātu.

Katru darbu prognozē atsevišķi.

> [!note] Piezīme
> Prognozi var veikt pēc vēsturiskajiem datiem, empīriska modeļa, pieredzes.
> Alternatīvi iespējams arī prognozēt darba "tilpumu". Tās būtu tādas metrikas kā pirmkoda rindas, funkcionālie punkti vai kas tml. 

Visas prognozes summē, lai iegūtu kopējo darbietilpību.

## Programmatūras vienādojums (Larry Putnam)

Šis ir dinamisks vairāku mainīgo vienādojums, ar kuru prognozēt darbietilpību.

$$\text{Darbietilpība}=\left[ \frac{\text{LOC} \cdot B^{0.333} }{P}\right]^3 \cdot \frac{1}{t^4}$$
$t$ – projekta ilgums mēnešos vai gados
$B$ – "īpašo prasmju reizinātājs"
$P$ – "produktivitātes parametrs"

## Programmatūras vienādojums (Lawrence Putnam)

$$\text{Darbietilpība} = \left[ \frac{\text{Apjoms}}{\text{Produktivitāte} \cdot \text{Laiks}^{4/3}} \right]^3 \cdot B$$


## Prognozēšanas precizitāte

Īsto programmatūras apjomu var zināt tikai kad projekts ir pabeigts.

Galvenie faktori, kas ietekmē gala apjomu ir:
- Atkārtota komponenšu lietošana
- Programmēšanas valoda
- Sistēmas izkliedētība

Ar laiku apjoma prognoze kļūst precīzāka.



# Darbietilpība un piegādes laiks

![[Pasted image 20240108143228.png]]

# Darbietilpības iedalījums

- 40-50% darbietilpības veltīts "priekšpuses" aktivitātēm
	- Komunikācija ar klientu
	- Analīze
	- Dizains
	- Analīze un mainīšana
- 15-20% veltīts veidošanas aktivitātēm
	- Kodēšana/programmēšana
- 30-40% veltīts testēšanai un uzstādīšanai
	- [[Definīcijas#Vienībtestēšana (Unit testing)|vienībtestēšana]]
	- [[Definīcijas#Baltās kastes testēšana (White-box tests)|baltās kastes testēšana]]
	- [[Definīcijas#Melnās kastes testēšana (Black-box testing)|melnās kastes testēšana]]
	- regresija


