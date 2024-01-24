
> [!info] Kas šis ir?
> Šis papildina [[Kvalitātes pārvaldība#Programmatūras kvalitāte un CMM (Capability Maturity Model)|CMM]] aprakstu ar metriku definīcijas standartu.

![[Pasted image 20240123122312.png]]

# Vispārējie dati![[Pasted image 20240123123141.png]]

![[Pasted image 20240123123141.png]]

# DCI piemēri

![[Definīcijas#DCI (Data Collection Item)]]

![[Pasted image 20240123123228.png]]
![[Pasted image 20240123123241.png]]

# Metriku kategorijas

## Uz mērķiem balstītas metrikas

Šīm metrikām jāseko visa projekta izstrādes laikā.
Jāizvirza kvantitatīvu mērķi un jāseko progress mērķa sasniegšanai.

## DCI

Šīs metrikas aprēķina no pieejamiem datiem.

# Metriku elementi

| Elements | Apraksts |
| ---- | ---- |
| Metrika | Metrikas nosaukums |
| Formula | Vienādojums, kas aprēķina metriku no mērījumiem |
| Mērījuma vienība | Mērījummu vienība, piem., [[Definīcijas#Pirmkoda rindas (Lines Of Code) (LOC)\|LOC]] |
| Apraksts | Ko metrika nozīmē un kā to izmantot |
| Vēlamais mērķis / ierobežojumi | Vēlamais kvantitatīvs mērķis, kā arī atļautās metrikas robežas.<br>Ja metrika ir tikai datu ievākšanas metrika, tai nebūs mērķa |
| Biežums | Cik bieži jāanalizē metriku dati.<br>**Ieteicams vismaz katras fāzes beigās un/vai ik pēc 3 mēnešiem** |
| Analīze | Apraksta analīzes procesus. |

# Metriku klasifikācija

## Izstrādes

Metrikas jaunai funkcionalitātes vai produkta izstrādei.

## Uzturēšanas

Dalīts uzlabojumu (darba veikšanai vajag vismaz 6 [[Definīcijas#Persondiena/Personmēnesis (Person-days/Person-months)|person-mēnešus]]) un atbalsta (vajadzīgas dažas stundas, parasti mazāk par 1 [[Definīcijas#Persondiena/Personmēnesis (Person-days/Person-months)|person-dienu]]) metrikās.

## Citi

Pārejas metrikas – kā informācija pāriet uz citu izstrādes komandu.

Funkcionālās verifikācijas testu – Kods atbilst funkcionālajām prasībām. Tā testē saskarnes un kļūdu apdari (error handling)

# Projekta dzīves cikls

1. Sākšana
2. Prasības
3. Dizains
4. Izstrāde
	- Programmēšana
	- Dokumentēšana
5. Vienībtestēšana
6. [[Testēšana]]
	- Integrācijas t.
	- Sistēmas t.
	- Akceptēšanas t.
7. Palaišana (Deployment)
	- Apmācības
	- Verifikācija
8. Noslēgums
	- Apskate
	- Klienta appmierinātība

# Izstrādes metrikas

## Darbietilpības prognozes novirze

Skat. [[Darbietilpība]]

$$ \text{Prognozes novirze} = \frac{\left(\text{Īstā darbietilpība}-\text{Darbietilpības prognoze}\right)}{\text{Darbietilpības prognoze}} \cdot 100\% $$

Šī metrika sniedz brīdinājumu ja projekta darbietilpība atšķiras no prognozētās. Ja novirze ir pietiekami liela, iespējams jāmaina [[Projektu plānošana#Laikplānošana|laikplāns]].

## Laikietilpības prognozes novirze

$$ \text{Prognozes novirze} = \frac{\left(\text{Īstā laikietilpība}-\text{Laikietilpības prognoze}\right)}{\text{Laikietilpības prognoze}} \cdot 100\% $$


Šī metrika sniedz brīdinājumu ja projekta laikietilpība atšķiras no prognozētās. Ja novirze ir pietiekami liela, iespējams jāmaina [[Projektu plānošana#Laikplānošana|laikplāns]].


## Fāzu darbietilpības izkliede

$$\frac{\text{Fāzes īstā darbietilpība}}{\text{Kopējā īstā darbietilpība}} \cdot 100\%$$


## Apjoma novirze

$$ \frac{\text{Kopējais apjoms}-\text{Kopējā apjoma prognoze}}{\text{Kopējā apjoma prognoze}} \cdot 100\%$$

## Produktivitāte

$$ \frac{\text{Kopējais apjoms}}{\text{Kopējā darbietilpība}} $$
Vienība: $\frac{\text{LOC}}{\text{Person-diena}}$ vai $\frac{\text{FP}}{\text{Person-diena}}$ vai $\frac{\text{DE}}{\text{Person-diena}}$

> [!question] WTF ir DE????

## Defektu blīvums

$$ \frac{\text{Defektu daudzums}}{\text{Kopējais apjoms}} $$
Vienība: $\frac{\text{Defektu skaits}}{\text{KLOC}}$ vai $\frac{\text{Defektu skaits}}{\text{FP}}$ vai $\frac{\text{Defektu skaits}}{\text{DE}}$

## Defektu atrisināšanas efektivitāte

$$\frac{D_{bd}}{D_{bd}+D_{ad}} \cdot 100\%$$
$D_{bd}$ – defektu skaits pirms piegādes
$D_{ad}$ – defektu skaits pēc piegādes


## Defektu atrisināšanas efektivitāte fāzē

$$ \frac{\text{Kopējais atklāto defektu daudzums fāzē}}{\text{Kopējais pirms-piegādes defektu skaits}} \cdot 100 \% $$

## Phase-wise defect detection rate

![[Pasted image 20240123133743.png]]
> [!info] I was too lazy to translate this

## Apskates efektivitāte

Skatīt
- [[Definīcijas#Apskate (Review)]],
- [[Definīcijas#Defekts (Defect)]]

$$ \frac{\text{Kopējie defekti apskatē}}{\text{Kopējie defekti, kas atklāti apskatē}+\text{Kopējie defiekti testēšanā}} \cdot 100 \% $$

## Pārtaisīšanas apjoms

$$ \frac{\text{Kopējā pārtaisīšanas darbietilpība defektu dēļ}}{\text{Kopējā darbietilpība}} \cdot 100 \% $$

## Pārtaisīšanas apjoms prasību maiņu dēļ

$$ \frac{\text{Kopējā pārtaisīšanas darbietilpība prasību maiņu dēļ}}{\text{Kopējā darbietilpība}} \cdot 100 \% $$

# Uzturēšanas metrikas

## Produktivitāte



$$ \frac{\text{Izpildīto darbu daudzums mēnesī}}{\text{Darbu kopējā darbietilpība}}$$

## Vidējais aprites (turnaround) laiks

$$ \frac{\sum_{i=1}^{n}{T_i}}{n} $$
Vienība: laiks uz vienu darbu

## Ietilpināšanās laikā

$$ \frac{\text{Piegādāto darbu daudzums laikā}}{\text{Piegādāto darbu daudzums}} \cdot 100 \% $$

## Piegādātie defekti

$$ \frac{\text{Piegādāto darbu daudzums ar defektiem}}{\text{Piegādāto darbu daudzums}} \cdot 100 \% $$

# Citas metrikas

![[Pasted image 20240123140138.png]]
![[Pasted image 20240123140150.png]]
