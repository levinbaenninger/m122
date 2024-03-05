# Eingabeumleitung

Als Eingabedaten können wir einem Befehl mit `<` Daten aus einer Datei schicken. Beispiel:

````Bash
nano datei.txt 

--- 

22
4
*
p
````

Nun können wir mit `<` den Inhalt der Datei für das Kommando `dc`, Taschenrechner, nutzen:

````Bash
dc < datei.txt
````

