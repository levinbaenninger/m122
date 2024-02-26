# Berechtigungen ändern

Mit dem Command `chmod` können wir die Berechtigungen ändern:

````Bash
chmod Benuzertyp+/-Berechtigung Datei/Ordner
````

## Benutzertypen

| Benutzertyp                 | Symbolischer Modus |
|-----------------------------|--------------------|
| Besitzer der Datei          | `u`                |
| Gruppe der Datei            | `g`                |
| Andere Benutzer             | `o`                |
| Besitzer, Gruppe und andere | `a`                |  

## Berechtigungen

| Berechtigung | Symbol | Zahlenwert |
|--------------|--------|------------|
| Lesen        | `r`    | 4          |
| Schreiben    | `w`    | 2          |
| Ausführen    | `x`    | 1          |

Dabei kann man auch mit den Zahlenwerten arbeiten:

````Bash
chmod 664 script.sh
````