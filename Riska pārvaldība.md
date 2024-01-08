![[Definīcijas#Risks (Risk)]]

**Risku pārvaldība** ietver risku [[#Risku klasificēšana|klasificēšanu]], [[#risku identificēšana|identificēšanu]], [[#Risku analīze|analīzi]], [[#risku plānošana|plānošanu]] un [[#Risku uzraudzība|uzraudzību]].

> [!info] Risku saknē ir sliktas prasības, prasību izmaiņas un grūtības paredzēt laiku un resursus.



# Risku klasificēšana

- [[#Projektu riski]]
- [[#Produktu riski]]
- [[#Biznesa riski]]

## Piemēri
| Risks | Ietekmē | Apraksts |
| ---- | ---- | ---- |
| Darbinieku maiņa | Projektu | Pieredzējuši darbinieki var pamest projektu |
| Pārvaldības maiņa | Projektu | Mainās organizācijas pārvaldība ar citiem mērķiem |
| Aparatūras trūkums | Projektu<br>Produktu | Aparatūru nevar piegādāt laikā |
| Prasību maiņa | Projektu<br>Produktu | Prasības mainās vairāk nekā domāts |
| Apjoma kļūda | Projektu | Projekts ir lielāks nekā domāts |
| [[Definīcijas#CASE\|CASE]] rīku spējas trūkums | Produktu | Atbalstošā programmatūra nedarbojas tik jaudīgi kā cerēts |
| Tehnolģiju izmaiņa | Biznesa | Tehnoloģijas kļūst novecojušas. |
| Produkta sācensība | Biznesa | Sācensis tiek izziņots pirms sistēmu pabeidz |

# Risku pārvaldības process
![[Pasted image 20240106183443.png]]
[[Riska pārvaldības process.canvas|Riska pārvaldības process (interactive canvas)]]


# Risku identificēšana
> [!info] Identificē projektu, produktu un biznesa riskus

Identificēšana var būt komandas aktivitāte vai balstīta uz projekta pārvaldītāja pieredzes.

Parasti dalās dažādu veidu riskos
- [[#Tehnoloģiju riski]]
- [[#Organizatoriskie riski]]
- [[#Cilvēku riski]]
- [[#Prasību riski]]
- [[#Aplēšu riski]]
- [[#Rīku riski]]

## Risku indikatori
| Riska veids | Indikatori |
| ---- | ---- |
| Tehnoloģiju | Vēla atbalsta aparatūras vai programmatūras piegāde. |
| Organizatoriskie | Bezdarbība no augšas, tenkas |
| Cilvēku | Vāja motivācija, sliktas attiecības komandā. Bieža darbinieku maiņa |
| Prasību | Biežas prasību maiņas, klientu sūdzības |
| Aplēšu | Nespēja iekļauties laika plānā. Nespēja tikt vaļā no defektiem |
| Rīku | Komandas nevēlēšanās lietot rīkus, sūdzēšanās par [[Definīcijas#CASE\|CASE]] rīkiem, vēlmes jaudīgākām darba stacijām. |


# Risku analīze
> [!info] Izpēta **iespējamību** un **sekas**

Iespējamība:
- ļoti zema
- zema
- vidēja
- augsta
- ļoti augsta

Risku sekas
- nenozīmīgas
- paciešamas
- nopietnas
- katastrofiskas

## Risku tabulas veidošana
| Risks | Iespējamība | Sekas | [[Definīcijas#RMMM\|RMMM]] |
| ---- | ---- | ---- | ---- |
|  |  |  |  |
|  |  |  |  |

## Draudu līmenis
![[Pasted image 20240106151844.png]]

## Atklātība pret risku sekām (RE, risk exposure)
$$
RE=P\cdot C
$$
$P$ - Iespējamība (Probability), ka risks izpildās
$C$ - Izmaksas[^1] projektam, ja risks izpildās


# Risku plānošana
> [!info] Veido plānu lai izvairītos vai mazinātu riska sekas

Katru risku jāapsver un jārada stratēģija riska pārvaldīšanai

## Izvairīšanās stratēģijas
> Samazina iespēju ka risks izpildās

## Atvieglināšanas (Minimization) stratēģijas
> Samazina/atvieglina sekas, produktam vai projektam, ja risks izpildās

## Ārkārtas (Contingency) plāns
> Plāns, ko darīt, kad risks izpildās.

## Piemēri

| Risks | Stratēģija |
| ---- | ---- |
| Organizatoriskās finansiālās problēmas | Sagatavot Dokumentu pārvaldībai, kas norāda kā projekts ietekmē uzņēmumu, tā mērķus un kāpēc vajadzīgs finansējums. Būtu jāparāda kā uzņēmumam budžeta samazināšana izmaksātu vairāk nekā alternatīva. |
| Darbaspēka algošanas problēmas | Paziņot klientam par potenciālām problēmām un kavējumiem, izpētīt ārēju komponenšu iepirkumus. |
| Darbinieku slimība | Pārorganizēt komandu, lai palielinātu zināšanu pārklāšanos, nodrošinot labāku darba sapratni starp darbiniekiem. |
| Defektīvas komponentes | Aizvietot defektīvās komponentes ar uzticamākām komponentēm. |
| Prasību maiņas | Izsekot potenciālām izmaiņām, lai izvērtētu ietekmi. |
| Organizācijas pārstrukturēšana | Gatavot dokumentu pārvaldībai, lai norādītu kā projekts palīdz sasniegt uzņēmuma mērķus. |
| Datubāzes jauda | Izpētīt augstākas jaudas risinājumus |
| Nenovērtēts izstrādes laiks | Izpētīt iepērkamas komponentes un izpētīt programmatūras veidošanas rīkus. |

# Risku uzraudzība
> [!info] Pārrauga riskus projekta izstrādes laikā

Vienmēr jāseko līdzi risku **iespējamības** un **seku** izmaiņām.

Galvenos riskus būtu jāapspriež pārvaldes progresa sanāksmēs.

# Risku mazināšana (mitigation)
Ja radušās nopietnas problēmas izstrādes procesā, jāuzsāk risku mazināšana lai novērstu katastrofālu projekta neizdošanos.

Vienlaicīgi arī [[Projektu plānošana|jāpārplāno]] projekts. Tas var nozīmēt pārrunas ar klientu par projektu un [[Definīcijas#Nodevumi (Deliverables)|nodevumiem]]. Jāveido jauns [[Projektu plānošana#Laikplānošana|laikplāns]] un jāvalidē ar klientu.

# Definīcijas, Paskaidrojumi
## Projektu riski
Ietver laika plānu un resursus 

## Produktu riski
Ietver kvalitāti un produkta jaudu

## Biznesa riski
Ietver organizatoriskos jautājumus veidojot programmatūru



## Tehnoloģiju riski
- Datubāze nespēj nodrošināt vajadzīgo jaudu
- Vairāklietojamās komponentēs ir defekti, kas neļauj tos lietot.

## Rīku riski
- Rīki nenodrošina vajadzīgo efektivitāti
- Rīki nav savietojami

## Organizatoriskie riski
- Pārstrukturēšana, ka projektam mainās pārvaldība
- Finansiālās problēmas, kas piespiež mainīt apjomu
## Cilvēku riski
- Nevar atrast pieredzējušu darbaspēku
- Svarīgs personāls nav pieejams
- Vajadzīgā apmācība nav pieejama

## Prasību riski
- Prasību maiņa pieprasa liela apjoma pārstrukturēšanu
- Klienti nesaprot prasību maiņu ietekmi uz projektu

## Aplēšu riski
- Kļūda aplēsēs, cik laika aizņem izstrāde
- Cik laika aizņem defektu labošana
- Programmatūras apjoma aplēses








[^1]: [[Projektu plānošana#Cena vai izmaksas|Atšķirība starp cenu un izmaksām]]
