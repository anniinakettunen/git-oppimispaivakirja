# Oppimispäiväkirja: Hajautettu git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet, jotka vaikuttivat tehtävän suorittamiseen?__

Vaikeinta oli hahmottaa ero paikallisen ja etärepositorion välillä sekä ymmärtää, miten haarat (`branch`) toimivat. Helpointa oli puskea paikalliset muutokset GitHubiin ja seurata, miten webissä tehdyt muutokset saadaan paikalliseen repositorioon `fetch` ja `merge` -komennoilla. Esteet selvisivät, kun testasin komentojen vaikutusta vaiheittain ja tarkistin aina `git status` ja `git branch` -komennoilla tilanteen.

-myös oli vaikea ymmärtää tarkoitettiinko tehtävässä, että piti kloonata Tehtava5 repositoria projektiin jossa oli kaikki kurssin tehtävät samassa vai kloonata kurssin tehtävät siihen tehtäva5 repoon. Kloonasin kurssin jo tehnyt tehtävät Tehtava5 repoon.
- linkki https://github.com/anniinakettunen/Harjoitus5

---

## Osiossa käyttämäni Git-komennot

| Komento | Kuvaus |
| --------| ------ |
| git status | Näyttää, mitä tiedostoja on muutettu |
| git add  | Lisää tiedoston staging-tilaan |
| git commit -m "viesti" | Tallentaa muutokset paikalliseen git-historiaan annetulla viestillä |
| git branch | Näyttää paikalliset haarat; voi luoda uusia haaroja |
| git checkout <haara> | Vaihtaa haaran toiseen haaraan |
| git fetch | Hakee muutokset etärepositoriosta mutta ei yhdistä niitä paikalliseen haaraan |
| git merge  | Yhdistää annetun haaran muutokset nykyiseen haaraan |
| git push | Puskee paikallisen haaran muutokset GitHubiin |
| git remote -v | Näyttää etärepositorion URL-osoitteet ja nimet |
