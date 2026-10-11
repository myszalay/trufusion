# Git Branch
## Prüfen, auf welchem Branch du bist

    git branch

Wenn du aktuell auf master bist, siehst du beispielsweise:
*master 

    git status

## Neuen Branch für deine Änderungen erstellen
    git switch -c laszlo        # neue Variante
    git checkout -b laszlo      # alte Variante

## Kontrolle
    git branch

## Branch Mergen
    git checkout main
    git pull origin main
    git merge laszlo
    git push origin main

## Prüfen, ob die Änderung auf dem Quellbranch überhaupt committet ist
    git checkout
    git status
    git log -n 5 --oneline

## Merge erzwingen
    git cherry-pick <COMMIT-ID>

## Branch löschen - Clean-up
    git branch -d laszlo