  

Valmis ohjelma sisältää:  
  

- Kirjautumissivun

- Rekisteröitymissivun

- Kotisivun (kaikki kirjat)

- Sivun jossa valitun kategorian kirjat

- kirjan tiedot (pop up)

- Tilintiedot

  

Henkilökunnalle:

  

- Asiakaslista

- lisää kirja

- Muokkaa kirjan tietoja

  

#### Aloittamatta:

- Sivun jossa valitun kategorian kirjat (yhdistä kotisivuun)

#### Kesken:

- Tilintiedot
- Kotisivun (kaikki kirjat) (click event problem)
- lisää kirjailija

#### Valmis:

- Tilintiedot
- Kirjautumissivu
- Rekisteröitymissivu
- kirjan tiedot (pop up)
- haku functio
- lisää kirja
- kirjan tietojen muokkaus

#### Bugit:

- [x] Kirjaudu ulos ei oikeasti kirjaudu ulos
- [x] Lainaukset eivät näy AccountDetails 
- [x] orderBy = "enimi, snimi DESC";    ei käännä järjestystä
- [x] ChangeValue avautuu tuhat kertaa
- [x] Vaihto ei päivitä AccountDetails ruutua
- [x] kirjan kansikuvaa voi painaa asiakkaana
- [ ] kirjan tiedot TB:t voi selectata asiakkaana
- [ ] duplicate key lainatessa
- [x] asiakas pääse asiakkaat ikkunaan oma tili ikkunasta
- [x] Oma tili menu ja footer lokaatiot pielessä
- [x] täytä molemmat kentät (tuki, palautteet)
- [x] Vaihda ja määritä tekstit väärissä kohdissa kun arvoja vaihdetaan.
- [x] loso ei voi määrittää
- [x] a-z
- [ ] Changevaluen placeholder toimii kunnes painetaan vaihda/määritä nappia

#### Tehtävät:

- [ ] Lisää kommentit
- [x] Lisää vaihda nappien toiminnot
- [x] Lisää ... jokaiseen kohtaan joka voi mennä yli label.width
- [x] tuki, palautteet, ehdota kirjaa pituus filtteröinti
- [x] estä vaihtaminen jos asnum jolla avataan accountDetails != User.asnum
- [x] Kun vaihdetaan käyttäjätunnusta, tarkistetaan ettei sitä ole jo käytössä
- [x] työntekijän työnimi muiden tietojen alapuolelle
- [x] Näytä vaihda napit vain jos käyttäjä contructor username == User.Username
- [x] poista työnimikkeen vaihda nappi
- [x] vaihda changevalue x nappi kuva
- [x] kirjan tiedot formatoitu huonosti, korjaa
- [x] lisää placeholderit changevalue formiin
- [x] Muokkaa userlist haku toimivaksi
- [ ] korjaa userlist autoscroll/forming koko kun haetaan

#### Esittely video:

- Login sivu: 
   - nimimerkki ja salasana filtterit
   - menu
   - tuki, 
   - palautteet
- Register
   - Filtterit
- Kotisivu
   - järjestys
   - haku
   - scrollaus
- BookInfo
  - Tee Lainaus
  - Muokkaa kirjan tietoja
  - poista kirja
  - katso onko se on hävinnyt home
- Lisää uusi kirja
  - Valitse kirjailija
  - Lisää tiedot ja lisää kirja
  - Katso että kirja ilmestyy home ikkunaan
- Lisää uusi kirjailija 
  - Kesken
- Oma tili 
   - Vaihda tietoja
   - Lainaukset
- Asiakkaat 
   - järjestys
   - näytä eri käyttäjien tiedot sekä lainaukset lainaukset
- Kirjaudu sisään eri asiakkaana
   - ei muokkaa tai poista nappeja
   - ei asiakkaat labelia
   - ei työnimikettä
- Kesken

-[[School]]
-[[Coding]]
