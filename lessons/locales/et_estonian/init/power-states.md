# Süsteemi olekud

## Tunni sisu

Seni veel ei ole näidatud süsteemi oleku käsurea kaudu konktrollimise viise. Seda teemegi nüüd. Kuid rääkides *init*ist räägime nii süsteemi käivitamise režiimidest kuid ka nendest, millega süsteemi peatada.

Süsteemi peatamiseks:

<pre>$ sudo shutdown -h now</pre>

Kuid võib kasutada ka sulgemise käsku:

<pre>$ sudo poweroff</pre>

See käsk lülitab süsteemi välja, ning täpsustama peab, millal see peab aset leidma. Lisada võib aja minutites, mille möödudes süsteem lõpetab töö.

<pre>$ sudo shutdown -h +2</pre>

Selline käsk lülitab süsteemi välja kahe minuti möödudes. *Shutdown* käsuga saab teostada ka taaskäivitamist.

<pre>$ sudo shutdown -r now</pre>

Kuid võib kasutada ka taaskäivitamise käsku:

<pre>$ sudo reboot</pre>

## Harjutus

Mõtiskleda, mis toimub *init*'iga süsteemi sulgemisel.

## Küsimus

Millise käsuga lülitatakse süsteem välja 4 minuti möödumisel?

## Vastus

*sudo shutdown -h +4*
