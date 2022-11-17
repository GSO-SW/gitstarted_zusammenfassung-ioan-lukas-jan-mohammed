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




