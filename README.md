# gitStarted Zusammenfassung
In diesem Repo soll zusammengefasst werden, was man für die Arbeit mit git und gitHub kennen sollte.
In [diesem cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) finden Sie Hinweise, wie man .md-Dateien formatiert.

## TODO
- Begriffe definieren und erklären (z.B. repository, branch etc.)
- git Befehle für die Arbeit mit lokalen Repositories (inkl. Erläuterungen)
- git Befehle für die Arbeit mit entfernten Repositories (inkl. Erläuterungen)

## TODO2
- Fachbegriffe OOP erklären (mit Beispielen)
  - abstract (Klassen) 
  -> Können nicht instanziiert werden, sondern nur an Kinder-Klassen vererbt werden. 
	Beispiel: 
	abstract class Mensch 
	{
	// Code
	}
	
  - abstract (Methoden)
  -> können nur innerhalb von abstact Klassen implementiert werden und müssen von erbenden, NICHT abstract, 
	 Klassen mit "override" einen Methodenkörper gegeben werden.
	 Beispiel für den Methodenkopf:
	 public abstract void InformationenAusgeben();
	 
  - virtual
  -> virtual methoden haben einen Methodenkörper und können von erbenden Klassen mit "override" einen
	 anderen Methodenkörper gegeben werden.
	 Beispiel:
	 public virtual string InformationenAusgeben()
	 {
		Console.WriteLine("Lorem Ipsum");
	 }
	   
  - override
  -> kann bei geerbten virtual methoden und muss bei geerbten abstract methoden verwendet werden, um diesen
     einen eigenen Methodenkörper zu geben.
	 Beispiel:
	 public override string InformationenAusgebenAusgeben()
	 {
		Console.WriteLine("Lorem Ipsum.");
	 }
	 
  - Polymorphie
  -> Unterschiedliche Klassen können in der gleichen Liste gespeichert werden, weil sie alle
	 von der gleichen Eltern-Klasse erben.
  
- Wie überschreibt man die Methode `virtual string ToString()`?
-> mit dem Schlüsselwort "override":
	public override string ToString()
	{
		return "Lorem Ipsum";
	}
	
	
	