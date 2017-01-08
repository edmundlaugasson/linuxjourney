# Omandiõigused

## Tunni sisu

Lisaks ligipääsuõigustele saab muuta ka faili omanikku: kasutajat ja gruppi.

<b>Omaniku muutmine</b>

<pre>
$ sudo chown peeter minufail
</pre>

See muudab faili omanikuks Peetri.

<b>Grupi muutmine</b>

<pre>
$ sudo chgrp vaalad minufail
</pre>
või ka
<pre>
$ sudo chown :vaalad minufail
</pre>

See muudab faili grupiks vaalad.

<b>Kasutaja ja grupi üheaegne muutmine</b>

Kui lisada kasutaja järele koolon ning grupinimi, saab neid üheaegselt muuta.

<pre>
$ sudo chown peeter:vaalad minufail
</pre>

## Harjutus

Muutke mõne testfaili omanikku, kasutajaid ja gruppi. Pärast aga vaadake õigusi käsuga *ls -l*.

## Küsimus

Millise käsuga saab muuta faili omanikku?

## Vastus

*chown*
