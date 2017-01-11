# Tuuma otsiteekond

## Tunni sisu

Mis juhtub  uue tuuma paigaldamisel? See lisab süsteemi mõned failid, mis tavaliselt paiknevad */boot* kataloogis.

Erinevate versioonide jaoks on mitmeid faile:

<ul>
<li><i>vmlinuz</i> - linuxi tuum</li>
<li><i>initrd</i> - ehk on veel meeles, initrd on ajutine failisüsteem, mida kasutatakse enne tuuma laadimist</li>
<li><i>System.map</i> - sümbolite tabel </li>
<li><i>config</i> - tuuma sätted, tuuma ise kompileerides, võib sätestada, milliseid mooduleid laetakse</li>
</ul>

Kui */boot* kataloogis saab ruum otsa, võib alati nende failide vanu versioone eemaldada kasutades selleks paketihaldurit. Selles kaustas hooldustööde tegemisega tasub olla ettevaatlik, et ei kustataks kogemata kasutusel olevat tuuma.

## Harjutus

Avage */boot* kataloog ja uurige seal asuvaid faile.

## Küsimus

Kuidas nimetatakse tuuma kujutist */boot* kataloogis?

## Vastus

*vmlinuz*
