# Ausgabeumleitung

Eine Ausgabe kann mit `>` in eine Datei gelenkt werden:

````Bash
grep -e vmuser /etc/passwd > datei.txt
````

Die Ausgabedatei wird neu angelegt, falls sich noch nicht vorhanden ist. Ansonsten wird sie neu beschrieben.

Wenn die Ausgabe lediglich angehängt werden soll, kann man `>>` verwenden:

````Bash
date >> datei.txt
````

## Trennung von Fehlerausgabe und Output

Linux trennt den Standard-Output und die Fehlerausgabe in die Kanäle 1 und 2 ein. Mit diesem Wissen lässt sich die Ausgabe filtern:

````Bash
find / -name "*usb*.conf" 2 > /dev/null
````

Hier wird die fehlerhafte Ausgabe in eine virtuelle Gerätedatei geschrieben.

