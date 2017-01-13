# Kenadus

## Tunni sisu

Kui tegeleda arvutis mitmete asjadega: korraga on avatud ehk Chromium, LibreOffice Writer ja GIMP siis vőib tunduda, et need protsessid töötavad kőik samal ajal, kuid tegelikult see päris nii ei ole.

Protsessid kasutavad protsessorit ainult väikese osa ajast, seda nimetatakse *time slice* ehk *ajakild, ajapilu*. Seejärel nad peatuvad millisekunditeks ja teised protsessid saavad oma ajapilu jagu aega. Vaikimisi toimub see ikka üksteise järel uuesti ja uuesti. Kőik protsessid saavad piisavalt ajavahemikke, kuni nad oma tööga valmis saavad. Tuum haldab kogu seda protsesside ümberlülitumist ja suurem osa ajast teeb seda ka väga edukalt. Protsessor töötab, nagu öeldakse, ajajaotusreziimis.

Protsessid ise ei saa otsustada millal ja kui palju nad protsessori aega kasutada saavad. Kui kőik töötavad tavapäraselt, saavad nad kőik ka (enamvähem) vőrdselt protsessori aega. On aga vőimalus tuuma protsessi vaikimisi algoritmi muutmiseks *nice*(tőlkes *kena*) väärtusega. Kenadus on küll veider nimi, kuid see tähendab, et protsessid saavad numbri, mis määrab nende prioriteedi protsessori jaoks. Suurem number tähendab, et protsess on "kenam" ja tal on madalam prioriteet protsessori jaoks, väike vői negatiivne number tähendab, et protsess ei ole väga kena ja tahab saada nii palju protsessori aega kui vőimalik. Kenaduse asemel võiks mõelda ka inimlikusest omadusest - "vastutulelikkusest" või "taanduvusest", mis oleks rohkem tehniline mõiste.

<pre>$ top</pre>

Tulp NI ongi protsessi kenaduse tase.

Kenaduse taseme muutmiseks vőib kasutada *nice* ja *renice* käske:

<pre>$ nice -n 5 apt upgrade</pre>

*Nice*i kasutatakse uuele protsessile prioriteedi määramiseks. *Renice* muudab aga juba olemas oleva protsessi prioriteeti.

<pre>$ renice 10 -p 3245</pre>

## Harjutus

Millised protsessid ei ole eriti kenad ja miks?

## Küsimus

Kui on vaja anda protsessile kõrgem prioriteet protsessori jaoks, kas *nice* number peab olema suurem vői väiksem?

## Vastus

väiksem
