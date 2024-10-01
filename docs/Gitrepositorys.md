# 1. Eine MkDocs-Dokumentation mit Hilfe von Git aus einem Repository laden

Um eine MkDocs-Dokumentation aus einem Git-Repository zu laden, benötigst du zuerst Git auf deinem System. Wenn du Git noch nicht installiert hast, kannst du es von [git-scm.com](https://git-scm.com/) herunterladen. Sobald Git installiert ist, öffne das Terminal oder die Eingabeaufforderung. Verwende den Befehl `git clone <URL-zum-Repository>`, um das Repository zu klonen, wobei du `<URL-zum-Repository>` durch die tatsächliche URL des MkDocs-Repositorys ersetzt. Nachdem der Klonvorgang abgeschlossen ist, wechsle in das neu erstellte Verzeichnis mit `cd <Name-des-Repositorys>`.

Falls du MkDocs noch nicht installiert hast, kannst du dies mit `pip install mkdocs` nachholen. Um die Dokumentation lokal anzuzeigen, starte den lokalen Server mit dem Befehl `mkdocs serve`. Du kannst die Dokumentation dann im Webbrowser unter `http://127.0.0.1:8000` aufrufen. Mit diesen Schritten kannst du die MkDocs-Dokumentation erfolgreich aus einem Git-Repository laden und lokal anzeigen.

# 2. Eine MkDocs-Dokumentation mit Hilfe von Git in ein Repository hochladen

Um eine MkDocs-Dokumentation in ein Git-Repository hochzuladen, musst du sicherstellen, dass alle Änderungen, die du an der Dokumentation vorgenommen hast, lokal gespeichert sind. Beginne damit, das Terminal oder die Eingabeaufforderung zu öffnen und in das Verzeichnis deiner MkDocs-Dokumentation zu navigieren. Um die Änderungen für das Commit vorzubereiten, führe den Befehl `git add .` aus, um alle Dateien hinzuzufügen. Anschließend kannst du mit `git commit -m "Meine Änderungen"` einen Commit erstellen und eine kurze Beschreibung der Änderungen hinzufügen.

Um die Änderungen nun in das Remote-Repository hochzuladen, verwende den Befehl `git push origin main`. Ersetze `main` durch den Namen des Branches, in den du die Änderungen hochladen möchtest, falls du einen anderen Branch verwendest. Nach dem Ausführen dieser Befehle wird deine MkDocs-Dokumentation erfolgreich in das Git-Repository hochgeladen und ist dort verfügbar.

# 3. Eine MkDocs-Dokumentation mit Hilfe von Git in ein Repository hochladen und automatisch als Webseite über Dienstanbieter veröffentlichen

Um eine MkDocs-Dokumentation zu erstellen und sie automatisch als Webseite zu veröffentlichen, kannst du GitHub Pages nutzen. Zuerst musst du ein neues Repository auf GitHub erstellen. Nachdem du dein Repository eingerichtet hast, generiere die Dokumentation mit dem Befehl `mkdocs build`. Dieser Befehl erstellt die statischen Dateien, die für die Veröffentlichung benötigt werden.

Wechsle danach in den `gh-pages`-Branch, indem du den Befehl `git checkout --orphan gh-pages` verwendest. Füge nun die generierten Dateien aus dem `site`-Verzeichnis hinzu, indem du `git --work-tree=site add --all` ausführst. Committe die Änderungen mit dem Befehl `git --work-tree=site commit -m "Veröffentlichung der MkDocs-Dokumentation"`. Um die Änderungen in den `gh-pages`-Branch zu pushen, verwende `git push origin gh-pages --force`.

Vergiss nicht, in den Einstellungen deines GitHub-Repositorys GitHub Pages zu aktivieren und den `gh-pages`-Branch als Quelle auszuwählen. Mit diesen Schritten wird deine MkDocs-Dokumentation automatisch als Webseite veröffentlicht, die über GitHub Pages zugänglich ist.

# 4. Den Git-Zugriff in den Editor als Schnellzugriff einbinden

Um den Git-Zugriff in einem Code-Editor wie Visual Studio Code als Schnellzugriff einzubinden, musst du sicherstellen, dass Git auf deinem Computer installiert ist. Öffne dann deinen Code-Editor und nutze das integrierte Terminal, um Git-Befehle direkt auszuführen. In Visual Studio Code kannst du das Terminal öffnen, indem du `Strg + `` (Grave Accent) drückst oder über das Menü "Terminal" ein neues Terminal öffnest.

Du kannst nun Befehle wie `git clone`, `git add`, `git commit` und `git push` direkt im Terminal eingeben, um mit deinem Git-Repository zu arbeiten. Darüber hinaus gibt es viele Git-Erweiterungen für Editoren, die eine grafische Benutzeroberfläche für Git-Befehle bieten. Suche im Erweiterungsmarkt deines Editors nach "Git" und installiere eine passende Erweiterung. Mit diesen Möglichkeiten kannst du den Git-Zugriff bequem in deinem Editor nutzen und deine Workflow-Effizienz steigern.

# Weitere Informationen:

Kommandozeile öffnen und git config ausführen. Dafür folgenden Befehl benutzen:  
`git config --global http.proxy http://kjs-04.lan.dd-schulen.de:3128`

Um die Datei nun zu klonen, folgenden Befehl benutzen:  
`git clone https://github.com/ACCOUNTNAME_EINTRAGEN/NAME_DES_REPOSITORYS_EINTRAGEN.git`

Um die lokale Datei nun wieder zurück zu pushen, folgenden Befehl benutzen:  
`cd NAME_DES_REPOSITORYS`  
`git add NAME_DER_DATEI.py`  
`git commit -m "Initial commit" NAME_DER_DATEI.py`  
`git push`

Nun ist die bearbeitete Datei wieder im Repository.
