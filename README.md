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

#### Mögliche Fehler "git branch"
Nach dem man einen Branch erstellt hat muss man den branch auschecken. Wenn das nicht gemacht wird, bleibt man auf dem Branch master und die Änderungen werden auf dem Master gespeichert. Dann brigt der Branch keinen Vorteil. 

### git merge 
"git merge"-Befehl wird benutzt um zwei Commits zusammenzuführen. Der daraus resultierende Commit hat dementspreschen als Elterncommit, zwei Commits. 

#### Mögliche Fehler "git merge"
Wenn man einen Branch mit dem master mergen möchte muss man auf dem master ausgecheckt sein und dann den Befehl ausführen mit dem name des Branches.

### git rebase
"git rebase" verändert die ganze Historie eines Branches. 

#### Mögliche Fehler "git rebase"
Die sintax von git rebase wird sehr oft mit dem sintax von git merge verwechselt. Um einen Branch in den andere zu überführen, muss man auf dem jenigen Branch ausgecheckt sein. Dann folgt der rebase Befehl mit dem Name des Branches wo der ausgecheckte Branch neue positioniert werden soll.  

### git log
Mit "git log" kann man sich die Commits eines Branches anzeigen lassen oder alles Commits zusammen. Um alle Commits sich anzeigen zu lassen muss man "git log --all" ausführen.

#### Mögliche Fehler "git log"
Oft benutzt man git log und möchte die Commits des Masters sehen. Jedoch tauchen nur Commits einens Branche. Das passiert wenn man auf ein Branch ausgecheckt ist, und nur git log benutzt. Um die Commits eines anderes Branches zu zeigen nutzt man der Befehl "git log" gefolgt von der Name des Branches

### git reset 
Der Befehl "git reset" schreibt die Historie neue. Der aktuelle Branch wird auf einem Älteren commit zurückgesetzt. 

#### Mögliche Fehler "git reset"
Wenn man einen reset durchführt, muss man aufpassen welche Hash-Wert man nehmt. Man soll sich vergewissern, dass der Hash-Wert auch der gewünschte ist.

### git cherry-pick
Der Befehl "git cherrypick" nehme nur einen einzelnen Commit raus ohne Historie. 

#### Mögliche Fehler "git cherry-pick"
Wenn man einen cherry-pick durschführt, muss man aufpassen welche Hash-Wert man nehmt. Man soll sich vergewissern, dass der Hash-Wert auch der gewünschte ist.

### git add
Der Befehl "git add" verschiebt alle geänderten Dataien im Staging-Area. Mit "git add *" werden alle Änderungen in Staging-Area übernohmen

#### Mögliche Fehler "git add"
Es soll aufgepasst werden, welche Dataien im Staging-Area sich befinden.

###git checkout
Der Befehl "git checkout" wechselt zwischen den Commits und Branches hin und her. 

#### Mögliche Fehler "git checkout"
Es soll aufgepasst werden auf welche Branch oder Commit man auschecken möchte. 


<<<<<<< HEAD
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


## Begriffe definieren und erklären:
- Repository      : Unter Repository versteht man ein Projekt.
- Branch          : Branch sind verweise auf ein Snapshot von deiner letzten Veränderung
- Stagingarea     : Alle geaddeteten Dateien sind auf der "Bühne" und können mit einem Commit zusammengefasst werden
- Merge-Konflikte : Die entstehen dann, wenn zwei Personen eine Zeile in einer Datetei geändert haben oder ein Entwickler eine Datei löscht, während ein anderer diese ändert.


## Fachbegriffe OOP erklären
Abstract:Der abstract-Modifizierer gibt an, dass dem modifizierten Objekt eine Implementierung fehlt oder dass diese unvollständig ist.
Der abstract-Modifizierer kann für Klassen, Methoden, Eigenschaften, Indexer und Ereignisse verwendet werden.


Abstract (Klasse):

Eine abstrakte Klasse darf nicht instanziiert werden.
Eine abstrakte Klasse enthält möglicherweise abstrakte Methode und Accessoren.

abstract class main
{
    public abstract int GetArea();
}

Abstract (Methode):
Eine abstrakte Methode ist implizit eine virtuelle Methode.
Abstrakte Methodendeklarationen sind nur in abstrakten Klassen zulässig.
public abstract void Car(); 


Virtual: Das Schlüssel Wort Virtual wird züm ändern einer Methode, Eigenschaften,Indexer oder Ereignisdeklaration verwendet.

public virtual string Name { get; set; }

    
    private int _num;
    public virtual int Number
    {
        get { return _num; }
        set { _num = value; }
    }

Override: Das beschreibt eine Technik in der OOP, die es einer abgeleiteten Klasse erlaubt, eine eigene Implementierung einer von Muterklasse geerbten Methoden zu defenieren.

public override void Method()
{
base.Method();
// implementation
}


Polymorphie: Das ermöglicht, dass ein Bezeichner abhängig von seiner Verwendung Objekte unterschiedlichen Datentyps annimmt.
oder ist eine Eigenschaft, die immer im Zusammenhang mit Vererbung und Schnittstellen auftritt.
Beispiel .... Eine Methode ist polymorph, wenn sie in verschiedenen Klassen die gleiche Signatur hat, jedoch erneut implementiert ist.


public override string ToString(){}



>>>>>>> origin/mohammad

=======
>>>>>>> origin/ioan
