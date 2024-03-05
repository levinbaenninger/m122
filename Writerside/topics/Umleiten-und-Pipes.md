# Umleiten und Pipes

Für die Automatisierung ist es wichtig, dass die Befehle mit Dateien und Daten umgehen können:

- Konfigurationsdateien sollen beim Starten eingelesen werden.
    
- Die Ausgabe der Befehle sollen als Berichte für Protokollierungszwecke in Dateien gespeichert werden.
    
- Teilweise sind nur die Fehler-Ausgaben von Belang, tw. werden alle Ausgabendaten verlangt und tw. ist die Ausgabe ohne Fehlermeldungen auszugeben.
    
- Die erzeugten Daten sollen weiteren Befehlen ohne Zwischenspeicherung direkt zur Verarbeitung übergeben werden, womit mehrere Befehle «zusammengehängt» werden sollen.

## Beispiel

In folgendem Beispiel werden Pipes und Umleitungen genutzt:

````Bash
cd /home/vmadmin

tr ' ' ';' < blumenartkel.txt | grep -e Schnittblume | grep -w "lagernd" | cut -d ';' -f 3,4 | sort -rn -k 2,2 -t ';' > schnittblumen.csv

cat schnittblumen.csv
````

Hier wird zuerst jedes Leerzeichen durch ein Semikolon in der Datei <path>blumenartikel.txt</path>. Danach werden alle Zeilen ausgewählt aus der Ausgabe vor dem Pipe-Operator mit `Schnittblume`. Das Gleiche geschieht mit `lagernd`. Nun werden nur noch die 3. und 4. Spalten ausgegeben und anschliessend nach dem numerischen Wert der zweiten Spalte sortiert. Schliesslich wird die Ausgabe in einer `.csv`-Datei gespeichert.