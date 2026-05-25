# Tekoälyn kehittäminen ja kuvien käyttö

**Päivitetty viimeksi:** 25.5.2026
**Versio:** 1.0 (LUONNOS)

> **HUOMAUTUS:** Tämä on yksinkertaistettu työluonnos siitä, miten Hammashelppi käyttää
> kuva-aineistoa tekoälyn kehittämiseen. Terveydenhuollon kuvat ovat erityisiä
> henkilötietoja, joten teksti ja erityisesti suostumusmenettely on tarkistutettava
> tietosuojavastaavalla (DPO) ja lakimiehellä ennen käyttöönottoa.

---

## Lyhyesti

Kehitämme Palvelua ja siihen liittyvää tekoälypohjaista kuva-analyysiä. Se antaa
asiakkaalle alustavan arvion siitä, onko todennäköistä syytä ottaa yhteyttä
hammaslääkäriin. Tekoäly ei tee diagnoosia eikä hoitopäätöksiä eikä ohjaa hammaslääkärin
työtä.

Kehitystyössä voimme käyttää valokuvista tehtyjä löydöksiä ja kuva-aineistoa muun muassa
tekoälyn konenäön opettamiseen. **Aineisto käsitellään niin, ettei siitä voi tunnistaa
yksittäistä henkilöä** – tunnistetiedot poistetaan ennen kehityskäyttöä.

---

## Mitä tämä tarkoittaa

- **Mitä käytetään:** suun alueen valokuvia ja niistä tehtyjä löydöksiä (esimerkiksi
  havainto reiästä, tulehduksesta tai limakalvomuutoksesta).
- **Mihin:** Palvelun parantamiseen ja tekoälymallien opettamiseen, jotta kuva-analyysi
  tulee tarkemmaksi.
- **Miten suojataan:** aineistosta poistetaan nimi, yhteystiedot ja muut tunnistetiedot.
  Kehityskäytössä aineistoa käsitellään tunnisteettomana.
- **Mitä emme tee:** emme myy aineistoa, emmekä käytä sitä mainontaan tai
  henkilökohtaiseen profilointiin.

---

## Suostumuksesi (suositeltu malli)

> **Suositus:** Toteuta tämä erillisenä, vapaaehtoisena valintana (opt-in), joka on
> erotettu käyttöehtojen hyväksymisestä. Palvelun käytön ei tule edellyttää tämän
> suostumuksen antamista.

Ehdotettu suostumusteksti sovellukseen:

> ☐ Annan luvan käyttää lähettämiäni kuvia ja niistä tehtyjä löydöksiä tunnisteettomassa
> muodossa Hammashelpin palvelun ja tekoälypohjaisen kuva-analyysin kehittämiseen.
> Tiedän, että tämä on vapaaehtoista, se ei vaikuta saamaani hoitoon, ja voin peruuttaa
> luvan milloin tahansa asetuksista.

- Suostumus on **vapaaehtoinen** eikä vaikuta hoitoon.
- Voit **peruuttaa** suostumuksen milloin tahansa. Peruutus koskee tulevaa käyttöä;
  jo aitoon anonymisoituun aineistoon yhdistettyä kehitystyötä ei aina voida perua,
  koska aineistoa ei voida enää yhdistää sinuun.

---

## Tarkistettavat kohdat (ei julkaista – muistilista)

- [ ] **Anonymisointi vs. pseudonymisointi:** onko kuva-aineisto aidosti anonymisoitavissa?
      Kuvien kohdalla tämä on vaativaa; jos aineisto on tunnistettavissa, kyse on
      henkilötiedoista ja terveystiedoista (GDPR 9 art.).
- [ ] **Käsittelyperuste:** todennäköisesti nimenomainen suostumus (GDPR 9 art. 2 a)
      ja/tai sosiaali- ja terveystietojen toissijaista käyttöä koskeva laki
      (toisiolaki) ja Findata-menettely.
- [ ] **Opt-in-toteutus:** suostumus erotettava käyttöehdoista; helppo peruuttaa.
- [ ] **Tietosuojaseloste:** kuvaus kehityskäytöstä, säilytysajat, mahdolliset
      vastaanottajat ja siirrot.
- [ ] **Vaikutustenarviointi (DPIA):** todennäköisesti tarpeen erityisten
      henkilötietojen ja uuden teknologian vuoksi.
- [ ] **Mallien jakaminen / kolmannet osapuolet:** käytetäänkö ulkopuolisia
      kehityskumppaneita tai pilvipalveluja, ja millä sopimuksilla (käsittelysopimukset,
      siirrot EU/ETA:n ulkopuolelle).
