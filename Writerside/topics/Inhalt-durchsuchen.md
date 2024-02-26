# Inhalt durchsuchen

Um den Inhalt einer Datei zu durchsuchen, nutzen wir das Kommando `grep`:

````Bash
grep -e vmuser /etc/passwd
````

Hier suchen wir nach dem Muster `vmuser` im Verzeichnis `/etc/passwd`. Ein weiterer Schalter ist der `-c`, dieser unterdrückt die normale Ausgabe und gibt uns die Anzahl Zeilen pro Eingabedatei an, mit diesem Muster:

````Bash
grep -c vm /etc/passwd
````
