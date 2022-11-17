# gitStarted Zusammenfassung
In diesem Repo soll zusammengefasst werden, was man für die Arbeit mit git und gitHub kennen sollte.
In [diesem cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) finden Sie Hinweise, wie man .md-Dateien formatiert.

## TODO
- Begriffe definieren und erklären (z.B. repository, branch etc.)
- git Befehle für die Arbeit mit lokalen Repositories (inkl. Erläuterungen)
- git Befehle für die Arbeit mit entfernten Repositories (inkl. Erläuterungen)

## TODO2
- Fachbegriffe OOP erklären (mit Beispielen)


## OOP Begriffe
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


## Git Befehle
- Begriffe
  - repository (Ist praktisch ein Ordner oder ein Projekt wo dazu gehörige Dateien verwaltet werden)
  - branch (Eine Bezeichnung bzw. ein Namensschild welches auf einen commit zeigt)
  - staging area (Beinhaltet Dateien die commitet werden können, es können Dateien mit "git add ..." hinzugefügt werden)
  - commit (Sowas wie ein Lesezeichen welches einen bestimmeten Standpunkt des Projekts beinhaltet)
- Befehle für die Arbeit mit lokalen Repositories
  - git config <params> (Hiermit können bestimmte Parameter der Gitconfig bearbeitet werden)
  - git init (Initialisiert eine neune Repository)
  - git add <Dateiname(* für alle Dateien)> (Fügt Dateien der Staging Area hinzu um diese anschließend commiten zu können)
  - git commit -m "text" (Fügt der Repository einen neuen Commit hinzu)
  - git checkout <commit/branch> (Geht zu dem angegebenen Commit / Branch)
  - git merge <branch> (Fügt 2 Branches zu einem Commit zusammen)
  - git log (Zeigt den gesammten verlauf von der Repository an (commits, merges usw.))
  - git branch <branch-name> (Erstellt einen neuen Branch)
  - git diff <commit/branch> <commit/branch> (Zeigt die Unterschiede zwischen den 2 commits)
  - git status (Zeigt aktuellen Status / Zustand der Stagingarea)
  - git reset (...)
  - git cherrypick (...)
  - git rebase (...)
- Befehle für die Arbeit mit entfernten Repositorys
  - git clone <link> (Lädt die gesamte Repository runter)
  - git push (Lädt alle veränderungen in die Github Repository hoch)
  - git fetch (Lädt alle Dateien aus der bereits verknüpften Online Repository runter)
  - git pull (Macht im Grunde genommen das selbe wie "git fetch" nur dass die Dateien mit den Lokalen gemerged werden)
  - git revert (...)


## Config Befehle
git config --global user.name "[name]"
git config --global user.email "[email address]"
git config --global color.ui auto
