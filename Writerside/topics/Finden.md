# Suchen

Mit dem Befehl `find` können wir Dateien suchen bzw. finden.

## Dateiname bekannt

Wenn der Dateiname bekannt ist, können wir folgendes machen:

````Bash
find /home -name "datei.txt"
````

Dieses Kommando sucht im Ordner `home` nach eine Datei namens `.txt`.

## Dateiname unbekannt

Wenn der Dateiname unbekannt ist, können wir einige Spezialzeichen nutzen:

`*` - steht für eine beliebige Anzahl von beliebigen Zeichen
`?` - steht für ein beliebiges Zeichen
`[]` - Zeichen können eingegrenzt werden

### Beispiele

````Bash
find /home/vmadmin/ -name "datei*"
````

````Bash
find /etc/ -name rc?.d
````

````Bash
find /etc/ -name rc[2-3].d
````