# pwd (Print Working Directory)

## Tunni sisu

Linuxis on kõik organiseeritud failidena. Mida sügavamale Linuxi maailma tungida, seda paremini hakatakse seda mõistma. Hetkel pidagem see lihtsalt meeles. Kõik failid on organiseeritud hierarhilise kataloogipuuna. Failisüsteemi esimese kataloogi nimi on väga asjakohaselt juurkataloog. Juurkataloogis asub palju kaustu ja faile, milles omakorda asub veel kaustu ja faile jne. Näide, kuidas kataloogi puu võib välja näha:

<pre>/
|-- bin
|   |-- file1
|   |-- file2
|-- etc
|   |-- file3
|   `-- directory1
|       |-- file4
|       `-- file5
|-- home
|-- var
</pre>

Failide ja kataloogide puhul räägitakse nende asukohast. Kui oleks kaust nimega *home*, mille sees oleks *pete* nimeline kaust, mille sees omakorda oleks kaust *Filmid*, siis näeks selle asukoht välja järgmine: */home/pete/Filmid*. Lihtne, või mis?

Failisüsteemis, nagu ka reaalses maailmas, teeb navigeerumise oluliselt lihtsamaks, kui teatakse asukohta ja kuhu minna tahetakse. Selleks, et asukohta näha võib kasutada käsku *pwd* (*print working directory*). Tõlkes tähendab see käsk "kuva asukoha otsiteekond" ning see lihtsalt näitabki, millises kataloogis hetkel asutakse. Pane tähele, et asukoht algab juurkataloogist.


<pre>$ pwd</pre>

Kus kataloogis hetkel ollakse? Proovige järgi uurida.

## Harjutus

Selles peatükis harjust ei ole.

## Küsimus

Kuidas saad teada, millises kataloogis parasjagu ollakse?

##

pwd
