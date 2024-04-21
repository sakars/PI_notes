# ISTQB terminoloģija
*Testa gadījums* grupē saistītos testus. ISTQB tos sauc par *Testa komplektiem*.
*Tests*: ISTQB sauc par *Testa gadījumu*
`TEST()` - ISTQB Test case (Testa gadījums)


# Kāpēc vienībtesti
- Kods strādā kā sagaidāms
- Dokumentācija
- Pārtaisīšanas laikā nodrošina jaunu kļūdu neveidošanos
- Palīdz atrast kļūdas

# GoogleTest

Cool C un C++ bibliotēka

Izstrādāja *Google Testing Technology* komanda

Neveiksmīgo testu izpilde

Organizē saistītos testus testu komplektos

Strādā ar dažādiem kompilatoriem

Neapstājas pie pirmā kļūdainā testa

Seko līdzi visiem definētajiem testiem

Iespējams izmantot koplietojamos resursus testos

Pamatā xUnit arhitektūra

# Pamatjēdzieni

- **Apgalvojumi (Assertions)** - pārbauda vai patiess nosacījums
	- Veiksmīgs/neveiksmīgs/fatāli neveiksmīgs rezultāts
	- Lieto, lai pārbaudītu testējamā koda uzvedību
- Testi - lieto apgalvojumus, lai pārbaudītu testējamā koda uzvedību
- Testa komplekts - apvieno testus
- Testa bāzes klase *(test fixture class)* - lieto, lai apvienotu testos lietoto kopīgo kodu
- Testa programma - satur daudzus komplektus

# Apgalvojumi

`ASSERT_*` - fatāla kļūda
`EXPECT_*` - nefatāla kļūda

ar `<<` var pievienot kļūdas ziņojumu.

# Testu veidošana

`TEST()` definē testu

`TEST(KomplektaNos, TestaNos)`

>[!warning] Nosaukumos nevar būt `_`

# Atspējošana

Pieliekot `DISABLED_` testu atslēdz




