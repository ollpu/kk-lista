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


### Yleisiä ratkaisutapoja ja tietorakenteita
Jos et keksi ratkaisua tehtävään, yritä soveltaa ongelmaa johonkin näistä:

 - Segmenttipuu
 - Binäärihaku
 - Dynaaminen ohjelmointi


[Tulostettava versio listasta](https://gitprint.com/ollpu/kk-lista/blob/master/lista.md)
