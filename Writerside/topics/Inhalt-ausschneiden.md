# Inhalt ausschneiden

Einzelne Spalten lassen sich mit `cut` ausblenden. Während bei `sort` das Standardtrennzeichen das Leerzeichen war, ist es bei `cut` <shortcut>Tab</shortcut>. Somit müssen wir es mit dem Schalter `-d` explizit angeben:

````Bash
cut -d ' ' -f 1,3 blumenartikel.txt 
````

