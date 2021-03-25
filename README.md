# Oh_my_Git_Aufgaben
In dem Repository "Oh_my_Git_Aufgaben", werden Oh my Git Beispiel Aufgaben ins echte Leben übertragen

git config -- global user.email <Email>
git config -- global user.name <Name>

Benutzte Befehle:
git init <Name des Repositorys>
# Man erstellt ein Repository damit

### .txt datei in dem Ordner erstellt ###

git add <datei>
#Das fügt die besagte datei dem index zu

git commit -m <ein kommentar zu dieser version mit "" erstellen>
#Fügt ein Kommentar dieser Version zu.

git log
#Man sieht alle bisherigen commit's
	git log --graph
	# Zeigt den Graphen der Commits

git checkouts:
->->->->git checkout HEAD~n <dateiname>
	#n entspricht wie viele versionen man zurück springen will
->->->->git checkout <min. 4 Zeichen des HASH-wertes z.B."1d9d62ef" des commit's> <dateiname>
	#Man springt auf eine fürhere Version zurück.
->->->->git checkout master
	#Springt auf die aktuellste version zurück

git branch:
->->->->git branch <branchname> 
	#Erstellt einen weitern Entwicklungszweig
->->->->git branch
	#Zeigt alle verfügbaren Zweige an
->->->->git checkout <branchname>
	#Spring zum gesagten Entwicklungszweig
->->->->git merge <branchname>
	#Schmelzt Entwicklungszweig in aktuellen anderen ein
		git reset --merge <branch>
		Unmergt den besagten branch

git push:
	git push
	# Pusht diese Lokale Version Hoch zu Github (Vorausgesetzt es ist ein github link)
	
git pull
	git pull
	#Holt die aktuelle Version von Github runter (Vorausgesetzt es ist ein github link)

git clone
	git clone <Repository-Link>	
	# Klont den Repository, bei dir lokal rein

Wie man Sachen mit git visualiziert:
http://git-school.github.io/visualizing-git/#free


Wie wir das erstellt haben:

git clone https://github.com/Thomas910-Cheat/Oh_my_Git_Aufgaben
cd Oh_my_Git_Aufgaben
nano Test.txt
git add Test.txt
git commit -m "Zeile X"
git push                                 -- Um seine Lokale Datei hoch zu laden und alles andere drin

git pull                                 -- Um die Online Datei herunterzuladen und alles andere drin
