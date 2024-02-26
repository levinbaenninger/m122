# Verzeichnis löschen

Um ein Verzeichnis zu löschen, nutzen wir `rmdir`. Dieses Verzeichnis muss jedoch leer sein bevor es gelöscht werden kann:

````Bash
rmdir ordner1/
````

Um dieses mühselige Verhalten zu ändern, können wir wie bei Dateien das Kommando `rm` nutzen, jedoch mit dem Schalter `-r`. Dies löscht das Verzeichnis und jeglichen Inhalt darin:

````Bash
rm -r ordner1
````

