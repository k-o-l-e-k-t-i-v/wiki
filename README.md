wiki
====
all-purpose central wiki

_Kolektiv je otevřené sdružení tvůrců algoritmických vizuálů a elektronických hudebníků respektujících tradici live codingu, umělecké formy využívající živé psaní kódu, vytvářející nástroje pro zvuk a obraz přímo před zraky diváků._

Michal Cáb, GND, Kryštof Pešek, Jiří Rouš, Georgij Bagdasarov, Martin Blažíček, Petr Zábrodský, Erik Bartoš, Andrej Boleslavský.


https://soundcloud.com/algorave-iii/algorve-iii-neone

https://soundcloud.com/algorave-iii/code-for-lunch

http://sonicity.cz/cs/kolektiv-pradelna


howto
======

Synchronizace vsech repozitori se serverem (umistenych v jednom folderu),
skript "sync.sh" umisteny relativne.. 


```
#!/bin/sh
for i in `ls -p|grep "/"`; do echo "Syncing "$i"\n"; cd $i; git commit -am "`date` sync" ; git pull ; git push ; cd .. ; echo "------------------------\n" ; done
```
