# Berechtigungen

Mit `ls -l` können wir die Rechte sehen:

````Bash
-rwxrw-r-- 1 vmadmin vmadmin   20 Feb 20 13:19 helloWorld.sh
````

Hier sehen wir die verschiedenen Rechte ganz links. 

## Aufbau

### Ordner oder Datei

Das erste Zeichen steht dafür, ob es ein Ordner ist oder nicht: `d` oder `-`

### Besitzer

Die nächsten drei Zeichen stehen für die Rechte, welche der Besitzer hat. Der Besitzer ist der, mit dem erstem Namen in der Liste: `rwx` oder `---`.

### Gruppe

Die drei darauffolgenden Zeichen stehen für die Rechte, welche eine Gruppe hat. Die Gruppe ist die, nach dem Besitzernamen: `rwx` oder `---`.

### Restliche Nutzer

Die restlichen Nutzer, welche nicht in eine der oberen Kategorien fallen, haben die Rechte am Schluss: `rwx` oder `---`.

> Das `x` bei Ordnen, sagt aus, ob man den Ordner bspw. mit `cd` betreten kann