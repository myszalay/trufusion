## Git Branch
Date: `12.Okt.2026`

**Table of Content:**
[TOC]

### 1. Aktuellen Branch Prüfen
Überprüfe auf welchem Branch du bist:

    git branch
    
    laszlo
    * main

Wenn du aktuell auf master bist, siehst du beispielsweise:

    *master 

    git status

### 2. Neuen Branch erstellen
Ein neuen Branch erstellen und gleichzeitig wechseln:

    git switch -c laszlo        # neue Variante
    git checkout -b laszlo      # alte Variante

Kontrolle mit:

    git branch
    
### 3. Branch Mergen
Vorher mit `git status` prüfen, ob all Änderungen eingecheckt und commited sind. Danach muss zum `main` Bruch gewechselt werden, dann mit dem `pull` Befehl den aktuellen Stand holen und mit `merge`den Brunch zum `main` zusammenführen. Der letzte Schritt ist mit `push`, alles von lokal zu GitHub oder BitBucket hochzuladen.

    git checkout main
    git pull origin main
    git merge laszlo
    git push origin main

### 4. Prüfen, ob die Änderung auf dem Quellbranch committet ist
    git checkout
    git status
    git log -n 5 --oneline

### Merge erzwingen
    git cherry-pick <COMMIT-ID>

### 5. Branch löschen - Clean-up
    git branch -d laszlo
    
### Git Basics
[Git and GitHub](file:///Users/laszlo/Documents/Rocket/HTML_Documentation/Git%20Branch.html)
