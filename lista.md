# KK-lista

 - Overflow
  - Riittääkö 32-bittinen luku varmasti? Entä riittääkö edes 64-bittinen?
    - 32-bit signed: 2.1 * 10^9
    - 64-bit signed: 9.2 * 10^18
    - Ainoastaan `long long` on _varmasti_ 64-bittinen
  - Overflow bitshiftauksessa esim. `(1<<33)` pitäisi olla `(1LL<<33)`
 - Off-by-one-virhe
