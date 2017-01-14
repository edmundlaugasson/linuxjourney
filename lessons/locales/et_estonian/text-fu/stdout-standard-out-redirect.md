# stdout (Standard Out)

## Tunni sisu

Praeguseks oleme juba päris paljude käskude ja nende väljunditega tuttavaks saanud ja see viib meid ka edasi järgmise teemani: sisend/väljund vood. Sisestame järgmise käsu ja pärast arutame, kuidas see töötab:

<pre>$ echo Hello World > pähklid.txt</pre>

Mis juhtus? Kontrollige seda kataloogi, kus käsk käivitati ja olge valmis valmis selleks, et sealt leida fail nimega *pähklid.txt*. Kui sinna sisse vaadata, siis peaks seal leiduma tekst *Hello World*. Selle ühe käsuga toimus mitu tegevust, vaatame neid lähemalt.

Vaatame esimest osa:

<pre>$ echo Hello World</pre>

Me teame, et see trükib terminali (ekraanile) *Hello World*, aga kuidas? Protsessid kasutavad sisend-väljund voogusid, et võtta vastu sisendandmeid ja väljastada väljundeid. Vaikimisi võtab *echo* käsk sisendi (standardsisend ehk *stdin*) klaviatuurilt ja tagastab väljundi (standardväljund ehk *stdout*) ekraanile. Seepärast kuvatakse ekraanile *Hello World*, kui sisestada käsureale *echo Hello World*. Sisendi-väljundi ümbersuunamisega saame aga seda vaikimisi käitumist muuta, see annab meile failide osas suurema paindlikuse.

Vaatame, mis käsuga edasi juhtus:

<pre> > </pre>

*>* on ümbersuunamise operaator, mis laseb meil muuta seda, kuhu suunatakse standardväljund. See lubab meil suunata *echo Hello Worldi* väljundi ekraani asemel faili. Kui sellist faili veel olemas ei ole, siis kohe see samas ka luuakse. Kui see aga on juba olemas, siis kirjutatakse see üle ja senine sisu kaob jäjetult. (olenevalt kestast saab lisada käsule lipu, et sellist olukorda vältida).

Ja nii põhimõtteliselt *stdout* ümbersuunamine töötabki!

Ütleme aga, et me ei taha oma *pähklid.txt* faili üle kirjutada. Õnneks on selle jaoks ja olemas ümbersuunamise operaator, *>>*:


<pre>$ echo Hello World >> pähklid.txt</pre>

See lisab *Hello Worldi pähklid.txt* faili lõppu. Kui aga faili eelnevalt ei eksisteerinud, siis luuakse see, justnagu > ümbersuunamise puhulgi.


## Harjutus

Proovige neid käske:

<pre>
$ ls -l /var/log > minuväljund.txt
$ echo Hello World > rm
$ > mingifail.txt 
</pre>

## Küsimus

Millist käsku kasutada kui on vaja väljund lisada olemasoleva faili lõppu?

## Vastus

*>>*
