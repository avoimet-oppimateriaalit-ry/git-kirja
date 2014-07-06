# git submodule

Esiintyy muodoissa:

+ git submodule add _repo_ _nimi_
+ git submodule update
+ git submodule update --init

Submoduli tarkoittaa toisen repon lisäämistä alirepoksi. Vapaa matikka -projektissa esimerkki submodulista on repo [https://github.com/avoimet-oppimateriaalit-ry/avoimet-oppimateriaalit-ry/vapaa-matikka-commons.git](Vapaa matikka COMMONS), joka on submodulina kaikissa Vapaa matikka -kirjoissa nimellä _commons_.

Tätä submodulin lisäämistä vastaa siis komento `git submodule add https://github.com/avoimet-oppimateriaalit-ry/avoimet-oppimateriaalit-ry/vapaa-matikka-commons.git commons`.

Yhdellä repolla voi olla useita submoduleja.

Heti repon kloonaamisen jälkeen sen submodulit eivät vielä sisällä mitään, vaan ne täytyy initialisoida. Tämä onnistuu komennolla `git submodule update --init`.

Myöhemmin submodulin päivittyessä submodulin uuden version saa käyttöön komennolla `git submodule update`, joka lukee repon sisältämät referenssit ja hakee niiden mukaiset submodulien versiot. On siis tärkeää huomata, että submodulin versio viittaa aina commitiin, ei koskaan branchiin.
