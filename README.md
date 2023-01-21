# Datorarkitektur (del III) - Dataminnet
Tredje delen i en serie som behandlar CPU-konstruktion i mjukvara. 
En simulerad processor som baseras på mikrodator ATmega328P implementeras i terminalmiljö,
där klockpulser, in- och utdata implementeras via inmatning samt utskrift från terminalen.

Denna del behandlar dataminnet, primärt hur skrivning och läsning kan ske direkt till en specifik adress 
eller indirekt via en pekare (via tre 16-bitars register X, Y och Z). 

OP-koder ST (Store Indirect) samt LD (Load Indirect) lades till för läsning och skrivning till dataminnet med pekare.
Funktionsliknande makron high och low lades till för att direkt erhålla lägre och högre byte vid tilldelning av 
en 16-bitars adress till önskat pekarregister (som i praktiken utgörs av två 8-bitars register).
  
I efterföljande delar ska ytterligare OP-koder, stacken, ALU:n samt interrupt-implementering ska läggas till.

Filen "embedded_computer_system_part3_start_code.zip" innehåller startkoden, där ett temporärt dataminnet är
implementerat direkt i styrenheten.

Resterande filer utgörs av den färdiga implementeringen av dataminnet.

Se video tutorial här:
https://youtu.be/CFb0XbDLEP0
