# GitHub-Einführung
Eine kleine Einführung in GitHub und git für einen Hackathon an der Beuth Hochschule für Technik Berlin

## Lokales Repository erstellen
Erstellt im aktuellen Verzeichnis ein git Repository
> git init

### Übersicht ausgeben
Gibt für das aktuelle Repository den Status des aktuellen Branches
aus. Zum Beispiel welche Dateien im nächsten Commit enthalten sind
und welche nicht überwacht werden.
> git status

## Staging
Dateien zum Commit hinzufügen:
> git add [Name oder Dateipattern]

#### Beispiele:
Die Datei readme.md zum nächsten Commit hinzufügen:
> git add readme.md
Alle Dateien mit der Endung md zum nächsten Commit hinzufügen:
> git add *.md

Alle Änderungen zum Commit hinzufügen:
> git add --all

## Commit
Änderungen ins lokale Repository übernehmen "commiten":
> git commit -m "[Commit Nachricht]"
Die Commit Nachricht, welche mit dem Parameter -m angegben wird,
ist eine zusätzliche Information, welche beim wiederfinden
eines bestimmten Commits helfen kann.

Beispiel:
> git commit -m "Fixed issue 324"

## Staging & Commit
Führt ein Staging und Commit für alle Änderungen gleichzeitig aus
> git commit -a -m "[Commit Nachricht]"

Beispiel:
> git commit -a -m "Fixed issue 453"

## Push
Änderungen zum Remote (GitHub) übertragen:
> git push -u [RemoteShortName] [Branchname]

Beispiel:
> git push -u origin master

Zu allen konfigurierten Remote Servern die Änderungen übertragen:
> git push -u

## Fetch
Alle Daten (inklusive Branches) vom Remote ins lokale Repository
holen. Führt kein "merge" durch.
> git fetch [RemoteShortName]

Beispiel:
> git fetch origin

## Branches auflisten
Alle lokalen und remote (GitHub) Branches auflisten:
> git branch -v -a

## Einen Remote Branch holen und lokal auschecken
> git fetch [RemoteShortName]
> git checkout [BranchName]

Beispiel:
> git fetch origin
> git checkout my-new-feature

## Branch lokal anlegen
> git branch [BranchName]

Beispiel:
> git branch my-new-feature

## Branch auschecken (wechseln / aktivieren)
> git checkout [BranchName]

Beispiel:
> git checkout my-new-feature
