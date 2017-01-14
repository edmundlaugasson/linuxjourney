# /dev kataloog

## Tunni sisu

Seadmed vajavad arvutiga ühendamisel tavaliselt juhtprogramme, et korralikult töötada. Seadmete juhtprogrammidega saab tegeleda läbi seadmefailide või -sõlmede, mis on tegelikult lihtsalt erilised failid, kuigi näevad välja nagu tavalised failid. Kuna seadmefailid on just nagu tavalised failid, saab nendega tegutsemiseks kasutada programme nagu *ls*, *cat* jne. Seadmefaile hoitakse tavaliselt kataloogis */dev*. Kui seal sisestada *ls* võib näha suurt hulka erinevaid seadmefaile.

<pre>$ ls /dev </pre>

Mõnda seadet on siin kursustel juba kasutatud ka, näiteks */dev/null*. Ühes peatükis sai */dev/null*'ile saadetud väljund, tuum teab, kuidas rakendada seda seadet ja lihtsalt heidab sisend kõrvale, väljundit ei tagastata.

Kui varemalt taheti lisada süsteemi seadmeid, võidi lihtsalt lisada fail */dev* kataloogi ja ta sinna ka unustada. Kui nüüd hästi järgi mõelda siis selgub, miks see ei ole eriti hea meetod. */dev* kaust nimelt kuhjub täis staatilisi faile või seadmefaile, mida on juba ammu uuendatud, kasutamine lõpetatud vms. Seadmetele määratakse seadmefail sellises järjekorras, milliseses tuum nad leiab. Nii võib juhtuda, et iga kord kui süsteem taaskäivitada, on seadmel erinev seadmefail.

Õnneks enam sellist meetodit ei kasutata. Nüüd kasutatakse hoopis midagi muud, et lisada ja eemaldada seadmeid dünaamiliselt. Sellest räägitakse tulevates peatükkides.

## Harjutus

Uurida */dev* kausta sisu. Kas on märgata tuttavaid seadmeid?

## Küsimus

Kus hoitakse süsteemi seadmefaile?

## Vastus

*/dev*
