> [!info] Definīcija
> Darbietilpība (Effort) ir strādāšanas daudzums, kas vajadzīgs, lai pabeigtu [[Projektu plānošana#Aktivitāte darbs|darbu]]. To parasti mēra person-mēnešos (jeb mērvienībā *cilvēku skaits \* laiks, cik tie strādā*)


# Prognozēšana

## Agrākā pieredze

Ar agrāko pieredzi ir iespējams prognozēt darbietilpību. Šis nav uzticams veids un ir ļoti atkarīgs no pārvaldnieka pieredzes.

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
**COCOMO** (**CO**nstructive **CO**st **MO**del) jeb konstruktīvais izmaksu modelis (?) ir regresijas models, kas balstīts uz koda rindu skaita.

Šis modelis ir labi piemērots uzticamai izmaksu, laika, apjoma un darbietilpības un kvalitātes aprēķināšanai.

To oriģināli izveidoja Berijs Boēms (Barry Bohem) 1981. gadā. Tas ir balstīts uz 63 projektu pētījumu, kas to padara par vienu no vislabāk dokumentētajiem modeļiem.

Vienkāršais COCOMO
$$ \text{Darbietilpība}=a \cdot (\text{KLOC})^b$$
$$\text{Laiks}=a \cdot (\text{Darbietilpība})^d$$
$$\text{Vajadzīgais cilvēku skaits}=\frac{\text{Darbietilpība}}{\text{Laiks}}$$
KLOC - Kilorindas koda.

| Projekta veids | a | b | c | d |
| ---- | ---- | ---- | ---- | ---- |
| Organisks | 2.4 | 1.05 | 2.5 | 0.38 |
| Daļēji atdalīts (Semi-Detached) | 3.0 | 1.12 | 2.5 | 0.35 |
| Iegults | 3.6 | 1.20 | 2.5 | 0.32 |

**Organisks** – Komanda ir adekvāti maza un problēma ir labi saprotama, tikusi atrisināta agrāk un komandai ir izpratne par problēmu.

**Daļēji atdalīts** – projekta izmērs, komandas pieredze, zināšanas par problēmām ir starp Organisku un Iegultu. Tiem vajag papildus laiku, tie ir ne-triviāli, tiem vajag radošumu. Kā piemērs ir kompilatori un iegultās sistēmas.

**Iegults** – sarežģīts projekts, par kuru komandai ir maz zināšanu, tam vajag lielu radošumu. Šādai programmatūrai vajag lielu komandas izmēru, izstrādātājiem jābūt pieredzējušiem un radošiem, lai veidotu šāda līmeņa projektus.

### COCOMO II
COCOMO II ir prognozēšanas modeļu hierarhija.

- **Lietotņu kompozīcijas modelis** – tiek izmantots agrīnajos posmos, kad prototipē lietotāja saskarnes, plāno programmatūru, apskata jaudu, sistēmu mijiedarbību un tehnoloģijas briedumu.
- **Agrīnā dizaina posma modelis** – lietots, kad prasības ir nostabilizētas un pamata projekta arhitektūra ir nodibināta.
- **Pēc arhitektūras posma modelis** – lietots programmatūras izstrādes laikā
### Citi modeļi

$\text{Darbietilpība} = 5.2 \cdot (\text{KLOC})^{0.91}$ – Walstona-Fēliksa (Walston-Felix) modelis

$\text{Darbietilpība}=5.5+0.73 \cdot (\text{KLOC})^{1.16}$ – Beilija-Basili (Bailey-Basili) modelis

$\text{Darbietilpība}=5.288 \cdot (\text{KLOC})^{1.047}$ – Doty modelis, ja $\text{KLOC}>9$

### Funkcionālie punkti (Function points (Albrecht))

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



## Automatizētie rīki


