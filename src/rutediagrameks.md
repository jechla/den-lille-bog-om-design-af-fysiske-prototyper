# Rutediagram

Vi kan nu lave et rutediagram for låsen. Udgangspunktet er, at vi har en enkelt variabel, der kaldes "pstate" (program state). Den begynder i til 1. Dermed vil et overordnet rutediagram for den uendelige løkke se sådan ud:

![Flowchart](./assets/flow1.png)

Her er processerne under hver forgrening, en funktion.

Vi mangler dog at forklare, hvordan vi kan skifte tilstand. Det afhænger faktisk af, hvad vi får tilsendt fra nøglen. Vi forestiller os, at den kan sende "A", hvis døren er åben i 6 sekunder, der skiftes til. Den kan sende "B", hvis det er åben for altid. Og den kan sende "AB", hvis døren skal låses. Dermed er der nødt til også at være et rutediagram for modtagelsen af beskeder fra radioen. Det ser sådan ud:

![Flowchart](./assets/flow2.png)

Vi skal så huske, at både "åben i 6 sekunder" og "luk" skal skifte til tilstand 1. 