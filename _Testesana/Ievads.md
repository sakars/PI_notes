---
aliases:
  - Testēšana
---

# Kas?

![[Definīcijas#Tests (Test)]]

![[Definīcijas#Programmatūra (Software)]]

![[Definīcijas#Testēšana (Testing)]]

# Kāpēc?

- [[Definīcijas#Kvalitātes nodrošināšana (Quality assurance)|Kvalitātes nodrošināšana]]: Testēšana palīdz pārliecināties, vai programmatūra atbilst noteiktajām prasībām un kvalitātes standartiem un ir piemērota paredzētajiem mērķiem. 
- [[Definīcijas#Defekts (Defect)|Defektu]] noteikšana: testēšana palīdz identificēt problēmas, lai tās varētu novērst pirms [[Definīcijas#Programmatūra (Software)|programmatūru]] nodot lietotājam
- Lietotāju apmierinātība: nodrošinām, ka [[Definīcijas#Programmatūra (Software)|programmatūra]] darbojas kā klients gaida.
- Uzlabota ticamība: Testēšana uzlabo uzticamību un stabilitāti.
- Izmaksu ietaupījumi: defektu atrašana un labošana sākumā ir lētāka nekā vēlāk
- Atbilstība: testēšana panāk, ka programmatūra pakļaujas juridiskajām un regulatoru prasībām
- Konkurence: testi uzlabo kvalitāti rezultējoties kvalitatīvākā un konkurējošākā produktā

# Ko jāpanāk? (Testēšanas mērķi)

- Novērst defektus
- Pārbaudīt prasību izpildi
- Pārbaudīt testējamā objekta pabeigtību, vai darbojas kā lietotājs sagaida
- Sniegt priekšstatu par kvalitātes līmeni
- Atrast [[Definīcijas#Defekts (Defect)|defektus]]
- Nodrošināt iesaistītās personas ar info lēmumu pieņemšanai
- Nodrošināt līgumisko, juridisko, regulējošo prasību ievērošanu


| Integrācijas testēšana                               | Akcepttestēšana                                                                                                                       | Regresā testēšana                            |
| ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| Pārbauda defektu veidošanos, savienojot komponentes. | Vai produkts atbilst lietotāja prasībām (Akcepttestēšana neietilpst [[Definīcijas#Kvalitātes nodrošināšana (Quality assurance)\|QA]]) | Kvalitātes nodrošināšanai, nevis lietotājiem |
![[Pasted image 20240420141357.png]]

# Testēšanas ieguldījums

- **Dokumentācija**: Testētājus jāiesaista prasību pārskatīšanā vai lietotāju stāstu precizēšanā, jo tas ļauj ātrāk atklāt [[Definīcijas#Defekts (Defect)|defektus]].
- **Projektēšana**: Sadarbība ar projektētājiem uzlabo izpratni par projektu un kā to pārbaudīt. Plašāka izpratne par projektu samazina koda un testu defektu risku.
- **Izstrāde/programmēšana**: Testētāju sadarbība ar izstrādātājiem uzlabo izpratni par kodu, kā to pārbaudīt.
- **Akcepttestēšana**: Testētāju programmatūras [[Definīcijas#Verifikācija (Verification)|verifikācija]] un [[Definīcijas#Validācija (Validation)|validācija]] pirms uzstādīšanas produkcijā ļauj atklāt sistēmas [[Definīcijas#Atteice (Failure)|atteices]]. Tas palielina iespējamību, ka [[Definīcijas#Programmatūra (Software)|programmatūra]] atbilst ieinteresēto pušu vajadzībām.
# Atkļūdošana

Programmētāju [[Definīcijas#Kļūda (Error)|kļūdas]] rada [[Definīcijas#Defekts (Defect)|defektus]].
Testu izpilde atrod [[Definīcijas#Atteice (Failure)|atteices]], kas rodas [[Definīcijas#Defekts (Defect)|defektu]] dēļ. [[Definīcijas#Atkļūdošana (debugging)|Atkļūdošana]] labo [[Definīcijas#Defekts (Defect)|defektus]].
Testētāji atrod [[Definīcijas#Kļūme (Failure)|kļūmes]], programmētāji veic [[Definīcijas#Atkļūdošana (debugging)|atkļūdošanu]].

>[!info]
>Testēšana =/= Atkļūdošana




