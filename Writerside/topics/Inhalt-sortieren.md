# Inhalt sortieren

Mit dem Befehl `sort` können wir den Dateiinhalt sortieren. Wenn die Datei, die wir sortieren wollen Leerzeichengetrennt ist, dann können wir mit dem Schalter `-k` die Spalte angeben, nach welche wir sortieren wollen:

````Bash
sort -k 2 blumenartikel.txt 
````

Wenn die Datei aber ein anderes Trennzeichen hat, dann können wir das mit dem Schalter `-t` angeben:

````Bash
sort -t ":" -k 6 /etc/passwd
````

