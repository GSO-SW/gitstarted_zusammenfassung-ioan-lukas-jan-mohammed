# gitStarted Zusammenfassung
In diesem Repo soll zusammengefasst werden, was man für die Arbeit mit git und gitHub kennen sollte.
- In [diesem cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) finden Sie Hinweise, wie man .md-Dateien formatiert.
- Mit diesen [Generator](https://www.tablesgenerator.com/markdown_tables) können Sie Tabellen für Markdown erzeugen

:dart: Ziele:
1. Die Arbeit soll nicht im Browser stattfinden. Clonen Sie das Repo und arbeiten Sie lokal.
1. Hier gehts um Teamwork: Ich erwarte häufige Commits (+ häufiges pushen/pullen )

## TODO
- Begriffe definieren und erklären (z.B. repository, branch etc.)
- git Befehle für die Arbeit mit lokalen Repositories (inkl. Erläuterungen)
- git Befehle für die Arbeit mit entfernten Repositories (inkl. Erläuterungen)

## TODO2
- Fachbegriffe OOP erklären (mit Beispielen)
  - abstract (Klassen)
  - abstract (Methoden)
  - virtual
  - override
  - Polymorphie
- Wie überschreibt man die Methode `virtual string ToString()`?


## Lukas: 
- Begriffe definieren und erklären (z.B. repository, branch etc.)

## Mohammed:
- Fachbegriffe OOP erklären (mit Beispielen)

## Jan:
- git Befehle für die Arbeit mit entfernten Repositories (inkl. Erläuterungen)

## Ioan:
- git Befehle für die Arbeit mit lokalen Repositories (inkl. Erläuterungen)


## Git Befehle für die Arbeit mit entfernten Repositories:
- git clone   :   Kopiert das entfernte Repository auf das lokale Repository 
- git fetch   :   Holt neu angelegte Dateien vom entfernten ins lokas Repository
- git pull    :   Fetch + Merge in einem Befehl
- git push    :   Übergibt den Commit aus dem lokalen Repository ins entfernte Repository


## Git Befehle für die Arbeit mit lokalen Repositories:
- git init 
- git commit 
- git branch
- git merge
- git rebase
- git log
- git reset
- git cherry-pick
- git add
- git checkout

### git init
Der Befehl "git init" verändert der actuelle Verzeichniss in ein git repository. 

#### Mögliche fehler "git init"
Wir sehr oft vergessen und man wundert sich warum die git befehle nicht funktionieren.

### git commit 
Der Befehl "git commit" folgt meisten mit dem "-m" als Paramerter. -m Parameter ist zuständig für den Nachricht des Commits.

#### Mögliche Fehler "git commit"
-m parameter wird nicht benutzt. Dadurch geht VIM auf und man wind gefördert einen Nachricht mitzugeben. 

### git branch
"git branch"-Befehl wird benutzt um einen Branch zu erstellen. Ein Branch ist nicht anders als ein Namensschild. 

### git merge 
"git merge"-Befehl wird benutzt um zwei Commits zusammenzuführen. Der daraus resultierende Commit hat dementspreschen als Elterncommit, zwei Commits. 

### git rebase
"git rebase" verändert die ganze Historie eines Branches. 

### git log
Mit "git log" kann man sich die Commits eines Branches anzeigen lassen oder alles Commits zusammen. Um alle Commits sich anzeigen zu lassen muss man "git log --all" ausführen.

### git reset 
Der Befehl "git reset" schreibt die Historie neue. Der aktuelle Branch wird auf einem Älteren commit zurückgesetzt. 

### git cherry-pick
Der Befehl "git cherrypick" nehme nur einen einzelnen Commit raus ohne Historie. 

### git add
Der Befehl "git add" verschiebt alle geänderten Dataien im Staging-Area.

###git checkout
Der Befehl "git checkout" wechselt zwischen den Commits und Branches hin und her. 