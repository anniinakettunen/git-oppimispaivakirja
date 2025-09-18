# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä  1-3 oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

Vaikeinta tässä tehtävässä oli Vim-editorista poistuminen commit-viestin kirjoittamisen jälkeen. Sen sen eri tilat (insert, komentotila) ja poistumiskomennot kuten :wq ja :q! tuntuivat aluksi sekavilta. Kirjoitin ne myös usein väärin. 

Tehtävät olivat melko selkeitä ja vaikeuksia tuli vasta Vim-editorissa. Opin uutta, että add voi tehdä myös yksittäiselle tiedostolle. Ennen teina aina git add . eli lisäsin kaiken muutoksen. 

Opin myös miten poistetaan sekä että tallentamattomille tiedostoille ei käy mitään. 

# Oppimispäiväkirja: Tehtävä 4 – Ominaisuushaarat ja tyylit

**Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?**

Tehtävässä 4 opin käyttämään feature branches Gitissä. .    

Ominaisuushaaran luominen auttoi oppimaan, miten kehitystyö voidaan eristää päähaarasta ja testata muutoksia erikseen ennen yhdistämistä. Haarojen vaihtaminen ja sivun uudelleenlataus selaimessa auttoi näkemään muutokset käytännössä. Asia oli jo tuttua Ohjelmistoprojekti 1 -kurssilta eli käytännössä kertausta.   

**Miten selvitin esteet:**  
- käytin usein git status -komentoa
- ei ollut paljon esteitä

## Osiossa käyttämäni Git-komennot

git harjoituksien 1-3 logipätkä alusta ja lopusta: 

Date:   Fri Sep 5 20:15:31 2025 +0300

    luotu anniina ja ohjelma tiedostot

commit b61c9018b8eb2a67bb7d3e4acfe9340d7cb0596c
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:13:10 2025 +0300

    Poistettu tarpeeton tiedosto

commit c6ca4a25da3075782477dbc3619a2be845bf96b2
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:11:12 2025 +0300

    hello muutettu indexiksi

commit 1772a5cb8dd843111763aad2ca34ca6256cf4cbd
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:09:49 2025 +0300

    muokattu otsikko

commit 7a462db1a98649a784f31e4b9a389a03c1e2dc4c
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:08:38 2025 +0300

    hello.html lisätty

commit b31a443ea9ba47ae80c1a2de692cae1f57254f75
commit ec83a4c904d6e273962bd1be88f878972f69ad5a (HEAD -> main, origin/main)
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:15:31 2025 +0300

    luotu anniina ja ohjelma tiedostot

commit b61c9018b8eb2a67bb7d3e4acfe9340d7cb0596c
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:13:10 2025 +0300

    Poistettu tarpeeton tiedosto

commit c6ca4a25da3075782477dbc3619a2be845bf96b2
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:11:12 2025 +0300

    hello muutettu indexiksi

commit 1772a5cb8dd843111763aad2ca34ca6256cf4cbd
Author: Anniina Kettunen <anniina.kettunen@gmail.com>
Date:   Fri Sep 5 20:09:49 2025 +0300

    muokattu otsikko

                                 git add .
warning: in the working copy of 'return', LF will be replaced by CRLF the next time Git touches it
PS C:\Git-versionhallintakurssi> git add .
PS C:\Git-versionhallintakurssi> git commit -m "Tehtävän 4. testimuutokset"
[main 8e99d29] Tehtävän 4. testimuutokset
 7 files changed, 76 insertions(+)
 create mode 100644 loru.txt
 create mode 100644 resepti.txt
 create mode 100644 retinoli.txt
 create mode 100644 return
PS C:\Git-versionhallintakurssi> git revert 
usage: git revert [--[no-]edit] [-n] [-m <parent-number>] [-s] [-S[<keyid>]] <commit>...
   or: git revert (--continue | --skip | --abort | --quit)

    --quit                end revert or cherry-pick sequence
    --continue            resume revert or cherry-pick sequence
    --abort               cancel revert or cherry-pick sequence
    --skip                skip current commit and continue
    --[no-]cleanup <mode> how to strip spaces and #comments from message       
    -n, --no-commit       don't automatically commit
 7 files changed, 76 insertions(+)
 create mode 100644 loru.txt
 create mode 100644 resepti.txt
 create mode 100644 retinoli.txt
 create mode 100644 return
PS C:\Git-versionhallintakurssi> git revert
usage: git revert [--[no-]edit] [-n] [-m <parent-number>] [-s] [-S[<keyid>]] <commit>...
   or: git revert (--continue | --skip | --abort | --quit)

    --quit                end revert or cherry-pick sequence
    --continue            resume revert or cherry-pick sequence
    --abort               cancel revert or cherry-pick sequence
    --skip                skip current commit and continue
    --[no-]cleanup <mode> how to strip spaces and #comments from message
    -n, --no-commit       don't automatically commit
    --commit              opposite of --no-commit
    -e, --[no-]edit       edit the commit message
    -s, --[no-]signoff    add a Signed-off-by trailer
    -m, --[no-]mainline <parent-number>
                          select mainline parent
    --[no-]rerere-autoupdate
                          update the index with reused conflict resolution if possible
    --[no-]strategy <strategy>
                          merge strategy
    -X, --[no-]strategy-option <option>
                          option for merge strategy
    -S, --[no-]gpg-sign[=<key-id>]
                          GPG sign commit
    --[no-]reference      use the 'reference' format to refer to commits

PS C:\Git-versionhallintakurssi> git revert HEAD
hint: Waiting for your editor to close the file...

[main 4cf8534] :wqevert "Tehtävän 4. testimuutokset" :wq This reverts commit 8e99d29595f7d97cf569d456080bf4f62719870c. ok commit q A :wq:wq:wq:wq#
 7 files changed, 76 deletions(-)
 delete mode 100644 loru.txt
 delete mode 100644 resepti.txt
 delete mode 100644 retinoli.txt
 delete mode 100644 return




| Komento                  | Kuvaus                                                                 |
|--------------------------|------------------------------------------------------------------------|
| git status               | Näyttää työtilan: mitkä tiedostot on muutettu, lisätty jne.             |
| git add <tiedosto>       | Lisää tiedoston staging-tilaan, eli mukaan seuraavaan commit-viestiin. |
| git reset HEAD <tiedosto>| Poistaa tiedoston tilan, mutta ei peruuta muutoksia työtilassa. |
| git restore <tiedosto>   | Palauttaa tiedoston.          |
| git commit -m "viesti"   | Tallentaa muutokset Git-historiaan annetulla viestillä.         |
| git log                  | Näyttää commit-historian aikajärjestyksessä.                           |
| git push                 | Lähettää paikalliset commitit GitHubiin tai muuhun etärepositorioon.  |
| git merge                | Yhdistää esim. tyylit haaran muutokset main -haaraan  |
| git checkout main        | Vaihtaa päähaaraa.  |

