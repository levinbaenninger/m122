# Pipe

Mit der Pipe können wir Daten weitergeben, ohne dass eine Datei dazu nötig ist. Die Daten werden durch das Pipe-Symbol `|` direkt dem nächsten Befehl weitergegeben.

````Bash
cut -d ' ' -f 2,4 blumenartikel.txt | sort -n -k 2
````
