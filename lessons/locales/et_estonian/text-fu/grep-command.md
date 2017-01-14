# grep

## Tunni sisu

Grep on kõige tavalisem tekstitöötlemise käsk. See võimaldab otsida failist tähemärke või sõnesid, mis vastavad teatud mustrile. Kuidas toimida, kui tahetakse teada, kas mingi fail eksisteerib mingis konkreetses kataloogis või kas mingis failis asub otsitav sõne? Kindlasti ei hakka keegi kogu teksti läbi otsima, vaid kasutaks grep'i!

Kasutame näitena näide.txt faili:

<pre>$ grep rebane näide.txt</pre>

Peaks nägema, et *grep* leidis sõna *rebane* failist *näide.txt*

Saab otsida ka väike- ja suurtähedele mittetundlikku teksti, kui kasutada lippu *-i*.

<pre>$ grep -i mingimuster mingifail</pre>

Et veelgi paindlikkust lisada, võib *grep*'i kombineerida teiste käskudega kasutades | operaatorit.

<pre>$ env | grep -i Kasutaja</pre>

Nagu näha, on grep väga mitmekülgne. Mustris võib kasutada ka regulaaravaldisi:

<pre>$ ls /mingikat | grep '.txt$'</pre>

Peaks kuvama kataloogist "mingikat" kõik TXT-tüüpi tekstifailid.

## Harjutus

Ehk ollakse kuulnud käskudest *egrep* ja *fgrep*, need on nüüd vananenud ning asendatud käskudega *grep -E* ja *grep -F*. Lugege *grep*'i man lehekülge ja saate rohkem teada.

## Küsimus

Millist käsku kasutada, et mingit tähemärgi kombinatsiooni leida?

## Vastus

*grep*
