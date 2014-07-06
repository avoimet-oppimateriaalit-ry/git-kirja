# git config

Esiintyy muodoissa:

+ git config --global user.name _nimi_
+ git config --global user.email _sähkopostiosoite_

Näillä komennoilla määritetään gitin käyttäjä.

Nimen täytyy olla muodossa "Etunimi Sukunimi", esimerkiksi `git config --global user.name "Barack Obama"`

Annetun sähköpostiosoitteen täytyy löytyä GitHubin sähköpostiasetuksista, jotta commitit tunnistuvat oikein. Esimerkiksi, jos käyttäjä `obama` olisi antanut GitHubissa yhdeksi sähköpostiosoitteistaan osoitteen `president@whitehouse.gov`, voisi hän kirjoittaa `git config --global user.email president@whitehouse.gov`
