# head

## Tunni sisu

Oletame, et meil on väga pikk fail, meil on neid isegi mitu, mille hulgast valida, proovige cat /var/log/syslog. Peaksite nägema lehekülgede kaupa teksti.  Mis siis, kui piisab ainult paarist esimesest tekstifaili reast? Neid saab kuvada käsuga head. Vaikimisi näitab head käsk faili esimest 10 rida.

<pre>$ head /var/log/syslog</pre>

Saab ka muuta ridade arvu sobivaks. Näiteks soovime näha hoopis esimest 15 rida.

<pre>$ head -n 15 /var/log/syslog</pre>

Lipp -n esindab ridade arvu.

## Harjutus

Mida teeb järgnev käsk ja miks?

<pre>$ head -c 15 /var/log/syslog</pre>

## Küsimus

Millist lippu kasutada, kui on vaja muuta head käsuga vaadeldavate ridade arvu?

## Vastus

-n

