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
  - abstract (Methoden)
  - virtual
  - override
  - Polymorphie
- Wie überschreibt man die Methode `virtual string ToString()`?

## Git
- Begriffe
  - repository (Ist praktisch ein Ordner oder ein Projekt wo dazu gehörige Dateien verwaltet werden)
  - branch (Eine Bezeichnung bzw. ein Namensschild welches auf einen commit zeigt)
  - staging area (Beinhaltet Dateien die commitet werden können, es können Dateien mit "git add ..." hinzugefügt werden)
  - commit (Sowas wie ein Lesezeichen welches einen bestimmeten Standpunkt des Projekts beinhaltet)
- Befehle für die Arbeit mit lokalen Repositories
  - git init (Initialisiert eine neune Repository)
  - git add <Dateiname(* für alle Dateien)> (Fügt Dateien der Staging Area hinzu um diese anschließend commiten zu können)
  - git commit -m "text" (Fügt der Repository einen neuen Commit hinzu)
  - git checkout <commit/branch> (Geht zu dem angegebenen Commit / Branch)
  - git merge <branch> (Fügt 2 Branches zu einem Commit zusammen)
  - git 