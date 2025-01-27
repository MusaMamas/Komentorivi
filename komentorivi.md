## Tivistelmä
**Komentorivin käyttö**: "pwd" näyttää nykyisen hakemiston, "ls" listaa tiedostot, ja "cd" vaihtaa hakemistoa.
"less" mahdollistaa tiedoston selaamisen, ja putkimerkki ("|") yhdistää komentoja.

**Tiedostojen käsittely**: Luo hakemistoja: mkdir. Kopioi tiedostoja ja kansioita: cp -r. Poista tiedostoja ja kansioita: rm, varoen koska ei roskakoria.

**SSH ja etäkäyttö**: ssh avaa etäyhteyden. scp kopioi tiedostoja etäkoneeseen.

**Apu ja historiat**: "man" näyttää komentojen ohjeet. Käytä tabulaattoria täydennykseen ja nuolia historiassa navigointiin.

**Pakettienhallinta**: Päivitä: sudo apt-get update. Asenna ohjelmistoja: sudo apt-get install. Poista ohjelmia: sudo apt-get purge.

# Komentorivi

## Micro asentaminen

![Update](micro1.png)

Näyttää siltä, että suoritin komennon sudo apt-get update, mutta sain virheilmoituksia liittyen pakettien julkaisuihin. Virheilmoitukset kertovat, että julkaisujen tiedostot ovat vielä voimassa tulevaisuudessa (esim. 5 päivää 23 tuntia), mikä estää päivitysten soveltamisen. Tämä saattaa johtua siitä, että järjestelmän kellonaika ja päivämäärä ovat väärin asetettuja.
Korjasin ajat, ja toiminut hyvin. Seuraavassa kerrassa pitää olla enemmän tarkempi.

![Install](micro2.png)

Suoritin komennon sudo apt-get install micro tarkoituksena asentaa "micro"-ohjelma. Ohjelman asennuksen yhteydessä huomattiin, että sen mukana asennettaisiin myös lisäpaketti "xclip". Minulta kysyttiin, haluanko jatkaa asennusta, mutta valitsin vaihtoehdon "K" (keskeytä), joten asennus ei edennyt loppuun.

![Check](micro3.png)

Suoritin komennon micro --version tarkistaakseni "micro"-ohjelman version. Tuloste osoittaa, että asennettu versio on 2.0.11.

## Kolme uutta komentoriviohjelmaa
