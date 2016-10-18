# KK-lista

### Miksei koodi mene läpi?

 - Overflow
  - Riittääkö 32-bittinen luku varmasti? Entä riittääkö edes 64-bittinen?
    - 32-bit signed: 2.1 * 10^9
    - 64-bit signed: 9.2 * 10^18
    - Ainoastaan `long long` on _varmasti_ 64-bittinen
  - Overflow bitshiftauksessa esim. `(1<<33)` pitäisi olla `(1LL<<33)`
 - Off-by-one-virhe
 - Taulukon koko ja indeksointi
  - Hyvä tapa on määritellä taulukko hieman liian suureksi (esim. 101010 jos tarvitaan 10^5).
  - 0-indeksointi vai 1-indeksointi? Tehtävänannoissa on usein 1-indeksointi.
 - Reunatapaukset
  - Toimiiko koodi jos n=0 tai n=1?
  - Jos syötteen jokainen arvo on pienin/suurin mahdollinen?
 - Verkot
  - Onko verkko suunnattu vai ei?
  - Voiko verkossa olla erillisiä solmuja?
 - Koodi
  - Onko koodiin unohtunut debug printtejä?
    - Jos käyttää esim. `clog` tai `cerr` debug-tulosteeseen, niiden unohtuminen ei haittaa jos aika vaan riittää.
 - TLE?
  - Voiko koodi joutua loputtomaan silmukkaan?
  - Voiko dynaamisen ohjelmoinnin tilan esittää eri muodossa?
    - Saako jonkin tilan muuttujan johdettua jo tilassa olevista muuttujista?


### Yleisiä ratkaisutapoja ja tietorakenteita
Jos et keksi ratkaisua tehtävään, yritä soveltaa ongelmaa johonkin näistä:

 - Segmenttipuu
 - Binääri/ternäärihaku
 - Ongelman pilkkominen pienempiin osiin
  - Dynaaminen ohjelmointi
  - Divide and Conquer
 - Ongelman ratkaisu käänteisessä järjestyksessä (lopusta alkuun)
 - Brute force/Backtracking jos hakualue on tarpeeksi pieni
 - Kaavan löytäminen arvoja laskemalla
 - Ongelman esittäminen verkkona
 - Ongelman esittäminen geometrisesti

[Tulostettava versio listasta](https://gitprint.com/ollpu/kk-lista/blob/master/lista.md)
