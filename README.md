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
- Befehle:
- git clone   :   Kopiert das entfernte Repository auf das lokale Repository 
- git fetch   :   Holt neu angelegte Dateien vom entfernten ins lokas Repository
- git pull    :   Fetch + Merge in einem Befehl
- git push    :   Übergibt den Commit aus dem lokalen Repository ins entfernte Repository
- git revert  :   Lässt Änderungen ungeschehen machen (genau wie reset im lokalen Repository)
- git branch -m old_branch new_branch  :   Erstellt einen neuen Branch und kopiert die Commits aus dem alten Branch in den neuen.

- Hinweis auf typische Fehler:
- git pull, die eigene Datei darf nicht bearbeitet sein
- git push, bei ersten Push <- git push --set-upstream origin branch-name
- git fetch, achte darauf, dass du den richtigen Merge fetchst
- git revert, denk dran, den Commit zu wählen. z.B. git revert master^
- git branch -m, achte drauf, dass der Name des neuen Branches noch nicht existiert! 