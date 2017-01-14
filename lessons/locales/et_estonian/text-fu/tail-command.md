# tail

## Tunni sisu

Sarnaselt *head* käsuga, laseb käsk *tail* vaadata vaikimisi etteantud faili viimast 10 rida.

<pre>$ tail /var/log/syslog</pre>

JSamuti nagu head puhul saab muuta, mitut rida kuvatakse.

<pre>$ tail -n 10 /var/log/syslog</pre>

Teine hea variant on kasutada *-f* (*follow* ehk järgi) lippu. See jälgib faili jooksvalt ajas, kui see peaks kasvama. Proovige ja vaadake, mis juhtub.

<pre>$ tail -f /var/log/syslog</pre>

Kui süsteemi aktiivselt kasutada, muutub *syslog* fail pidevalt. *tail -f* käsu kasutamisega näeb kõike, mida sinna parasjagu lisatakse.

## Harjutus

Vaadake tail käsu *man* lehekülge ja uurige mõne käsu kohta, mida me ei tutvustanud.

<pre>$ man tail</pre>

## Küsimus

Millist lippu kasutakse faili jooksvaks jälgimiseks?

## Vastus

*-f*
