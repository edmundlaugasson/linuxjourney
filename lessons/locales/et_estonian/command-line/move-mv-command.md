# mv (Move)

## Tunni sisu

Seda käsku asutatakse failide liigutamiseks, aga ka ümbernimetamiseks. Lippude ja toimimise poolest on see käsule cp üsna sarnane.

Faile saab ümber nimetada nii:

<pre>$ mv vanafail uusfail</pre>

Faili võib liigutada hoopis teise kataloogi:

<pre>$ mv fail2 /home/pete/Dokumendid</pre>

...ja liigutada rohkem kui ühte faili korraga:

<pre>$ mv fail_1 fail_2 /mingikataloog</pre>

Katalooge saab ka ümber nimetada:

<pre>$ mv kataloog1 kataloog2</pre>

Nagu ka cp puhul, kui liigutada faili või kataloogi, siis see kirjutab samas kaustas teise samanimelise, mis seal võib juba olla, üle. Seega, kasutada -i lippu, et saaksid teate enne kui midagi üle tahetakse kirjutada.

<pre>$ mv -i kataloog1 kataloog2</pre>

Aga ütleme, et tahetakse liigutada faili just nimelt selliselt, et see kirjutaks eelmise üle. Failist võib teha varuvariandi, sel juhul nimetatakse vana fail ümber ~ sümboliga.

<pre>$ mv -b kataloog1 kataloog2</pre>

## Harjutus

Anda mõnele failile uus nimi, seejärel liiguta see teise kataloogi.

## Küsimus

Kuidas anda failile nimega *kass* uus nimi *koer*?

## Vastus

mv cat dog
