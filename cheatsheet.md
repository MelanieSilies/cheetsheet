##Terminal Cheat Sheet

Repositority öffnen: SSH Key aus Git hub kopieren -> `git clone SSHkey`

Order Erstellen: `mkdir`
Datei erstellen: `touch`
Löschen: `rm` (remove)
Anleitung zeigen: `man` (manual) -> verlassen mit "q"

---

`Open .` 
Öffnet das Verzeichnis im Finder 


Open (-e / -a / -t)
Mit den open-Befehlen können Sie Dateien oder Anwendungen vom Terminal aus öffnen.

Verwenden Sie `open -e` Dateiname, um eine Datei mit TextEdit 
(dem Mac-eigenen Textbearbeitungsprogramm) zu öffnen 
$~ open e mytext.txt

Verwenden Sie `open -a` Anwendungsname, um eine Anwendung wie TextMate oder Adobe Photoshop zu öffnen.
 $~ open a TextMate

Wenn ein Anwendungsname Leerzeichen enthält, kennzeichnen Sie diese Leerzeichen mit einem \, etwa so:
$~ open a Adobe\ Photoshop\ CS

Verwenden Sie `open -t`, um die Datei mit dem Standard-Texteditor zu öffnen (sofern es sich nicht um TextEdit handelt).
$~ open t myfile.rb

---

`Tap`-Taste
Automatisches Auslüllen der Ordnernamen

`q` Das sind exit Befehle. Wenn man zum Beispiel mit dem less Befehl eine Datei anzeigt, kann man mit q wieder zurück zur normalen Konsole springen. Oft, wenn man sonst nicht weißt wie man zu der normalen Konsole zurück kommt hilft ctrl+c . 

---

`ctrl + A` Gehe zum Anfang der Zeile, in der du gerade tippst
`ctrl  + E` Gehe zum Ende der Zeile, in der du gerade tippst
`ctrl  + U` Löscht die Zeile vor dem Cursor
`ctrl  + K` Löscht die Zeile nach dem Cursor
`ctrl  + W` Löscht das Wort vor dem Cursor
`ctrl  + T` Vertauscht die letzten beiden Zeichen vor dem Cursor
`Esc + T` Die letzten beiden Wörter vor dem Cursor vertauschen
`ctrl  + L` Löschen des Bildschirms
`ctrl  + C` Beenden des Programms, das Sie gerade ausführen
`ctrl  + D` Beenden der aktuellen Shell
`Option + →` Cursor ein Wort vorwärts bewegen
`Option + ←` Cursor ein Wort rückwärts bewegen
`ctrl  + F` Cursor ein Zeichen vorwärts bewegen
`ctrl  + B` Cursor ein Zeichen rückwärts bewegen
`ctrl  + Y` Einfügen, was mit dem letzten Befehl ausgeschnitten wurde
`ctrl  + Z` Setzt den Prozess, den Sie gerade ausführen, in einen angehaltenen Hintergrundprozess
`ctrl  + _` Rückgängig machen des letzten Befehls
`Option + Umschalt + Cmd + C` Einfachen Text kopieren
`Shift + Cmd + V` Einfügen der Auswahl
exit Beendet eine Shell-Sitzung

####Basics
`/` (Slash) Verzeichnis der obersten Ebene
`.` (Einfacher Punkt) Aktuelles Verzeichnis
`..` (Doppelter Punkt) Übergeordnetes Verzeichnis
`~` (Tilde) Heimatverzeichnis (alt+n)
`sudo [Befehl]` Befehl mit den Sicherheitsrechten des Superusers ausführen (Superuser do)
`nano [Datei]` Öffnet den Terminal-Editor
`open [Datei]` Öffnet eine Datei
`[Befehl] -h`  Holt Hilfe zu einem Befehl
`man [Befehl]` Zeigt das Hilfehandbuch des Befehls an
`Touch` erstellt eine neue Datei. Daran denken, der Datei die korrekte Endung zu geben. touch neuedatei.txt

---

####Change Directory - Verzeichnis wechseln
`cd` Heimatverzeichnis
`cd [Ordner]` Verzeichnis wechseln, z.B. cd Dokumente
`cd ~` Heimatverzeichnis
`cd/` Wurzel des Laufwerks
`cd -` Vorheriges Verzeichnis oder Ordner, den Sie zuletzt durchsucht haben
`pwd` Zeigt Ihr Arbeitsverzeichnis an
`cd..`	In das übergeordnete Verzeichnis wechseln
`cd../..`	Zwei Ebenen nach oben gehen

---

####List Directory Contents - Verzeichnisinhalt auflisten
`ls` Anzeige der Namen von Dateien und Unterverzeichnissen im Verzeichnis
`ls -C` Mehrspaltige Ausgabe der Liste erzwingen
`ls -a` Alle Einträge auflisten, einschließlich derer mit .(Punkt) und ..(doppelter Punkt)
`ls -1` Die Liste der Dateien im Format ein Eintrag pro Zeile ausgeben
`ls -F` Anzeige eines / (Schrägstrich) unmittelbar nach jedem Pfad, der ein Verzeichnis ist, * (Sternchen) nach ausführbaren Programmen oder Skripten und @ nach einem symbolischen Link
`ls -S` Dateien oder Einträge nach Größe sortieren
`ls -l` Liste in einem langen Format. Enthält Dateimodus, Eigentümer und Gruppenname, Datum und Uhrzeit der Dateiänderung, Pfadname und mehr
`ls -l /` Liste des Dateisystems von root mit symbolischen Links
`ls -lt` Auflistung der Dateien, sortiert nach Änderungszeit (neueste zuerst)
`ls -lh` Lange Auflistung mit menschenlesbaren Dateigrößen in KB, MB, oder GB
`ls -lo` Auflistung der Dateinamen mit Größe, Besitzer und Flags
`ls -la` Detaillierte Auflistung der Verzeichnisinhalte, einschließlich versteckter Dateien
`ls -al` Detaillierte Auflistung der Verzeichnisinhalte, einschließlich versteckter Dateien

---

####File Size and Disk Space - Dateigröße und Speicherplatz
`du` Nutzung für jedes Unterverzeichnis und dessen Inhalt auflisten
`du -sh [Ordner]` Menschenlesbare Ausgabe aller Dateien in einem Verzeichnis
`du -s` Anzeige eines Eintrags für jede angegebene Datei
`du -sk* | sort -nr` Auflisten von Dateien und Verzeichnissen, einschließlich der Größe der Unterverzeichnisse. Ersetzen Sie sk* durch sm*, um Verzeichnisse in MB aufzulisten
`df -h` Berechnen des freien Speicherplatzes auf Ihrem System
`df -H` Berechnet den freien Speicherplatz in Potenzen von 1.000 (im Gegensatz zu 1.024)

---

####File and Directory Management - Datei- und Verzeichnisverwaltung
`mkdir <ordner>` Neuen Ordner mit dem Namen <ordner> erstellen
`mkdir -p <ordner>/<ordner>` Verschachtelte Ordner erstellen
`mkdir <dir1> <dir2> <dir3>`` Mehrere Ordner auf einmal erstellen
mkdir "<ordner name>"` Erzeugen eines Ordners mit einem Leerzeichen im Dateinamen
`rmdir <ordner>` Löschen eines Ordners (funktioniert nur bei leeren Ordnern)
`touch <Datei>`` Eine neue Datei ohne Erweiterung erstellen
cp <Datei> <Verzeichnis>` Kopieren einer Datei in den Ordner
`cp <Datei> <neueDatei>` Kopieren einer Datei in den aktuellen Ordner
`cp <Datei>~/<Verzeichnis>/<NeuDatei> `Kopieren einer Datei in das Verzeichnis und Umbenennen der kopierten Datei
`cp -R <ordner> <"new dir">` Kopiert einen Ordner in einen neuen Ordner mit Leerzeichen im Dateinamen
`cp -i <Datei><Verzeichnis>` Fordert Sie vor dem Kopieren einer Datei mit einer Überschreibungswarnung auf
`cp <Datei1> <Datei2> <Datei3>/Benutzer/<Verzeichnis>` Kopieren mehrerer Dateien in einen Ordner
`ditto -V [Ordnerpfad][neuer Ordner]` Kopiert den Inhalt eines Ordners in einen neuen Ordner. Hier gibt "-V" für jede kopierte Datei eine Statuszeile aus
`rm <Datei>` Löschen einer Datei (Dies löscht die Datei dauerhaft; mit Vorsicht verwenden.)
`rm -i <Datei>` Eine Datei nur löschen, wenn Sie eine Bestätigung geben
`rm -f <Datei>` Erzwingen des Löschens ohne Bestätigung
`rm -R <ordner>` Löschen eines Ordners und seines Inhalts
`rm -rf <order>` Löscht ohne bestätigung (Achtung, kann auch schief gehen. Nut nutzen, wenn 100% sicher. Wenn weg, dann wirklich weg!
`rm <Datei1> <Datei2> <Datei3>` Mehrere Dateien ohne Bestätigung löschen
`mv <Datei> <NeuerDateiname>` Verschieben/Umbenennen
`mv <Datei> <Verzeichnis>` Verschieben einer Datei in den Ordner, möglicherweise durch Überschreiben einer vorhandenen Datei
`mv -i <Datei> <Verzeichnis>` Optionales Flag -i zur Warnung vor dem Überschreiben der Datei
`mv *.png ~/<ordner>` Verschiebt alle PNG-Dateien aus dem aktuellen Ordner in einen anderen Ordner

---

####Befehlsverlauf
`ctrl + R` Durchsuchen der zuvor verwendeten Befehle
history n Zeigt die vorhergehenden Befehle an, die Sie eingegeben haben. Fügen Sie eine Zahl hinzu, um die letzten n Einträge zu begrenzen
`![Wert]` Führt den zuletzt eingegebenen Befehl aus, der mit einem Wert beginnt
`!!`	Führt den zuletzt getippten Befehl aus

---

####Berechtigungen
`ls -ld` Zeigt die Standardberechtigung für ein Home-Verzeichnis an
`ls -ld/<ordner>` Anzeige der Lese-, Schreib- und Zugriffsrechte für einen bestimmten Ordner
`chmod 755 <Datei>` Ändern Sie die Berechtigung einer Datei auf 755
`chmod -R 600 <ordner>` Ändern Sie die Berechtigung eines Ordners (und seines Inhalts) auf 600
`chown <Benutzer>:<Gruppe> <Datei>` Ändern Sie den Besitz einer Datei auf den Benutzer und die Gruppe. Fügen Sie -R hinzu, um den Inhalt eines Ordners einzuschließen

---

####Prozesse
`ps -ax` Ausgabe der aktuell laufenden Prozesse. Dabei zeigt a die Prozesse aller Benutzer und x die Prozesse an, die nicht mit dem Terminal verbunden sind
`ps -aux` Zeigt alle Prozesse mit %cpu, %mem, page in, PID und Befehl
`top` Zeigt Live-Informationen über aktuell laufende Prozesse an
`top -ocpu -s 5`` Anzeige der Prozesse sortiert nach CPU-Auslastung, Aktualisierung alle 5 Sekunden
top -o rsize` Sortieren der Prozesse nach Speicherauslastung
`kill PID` Beendet den Prozess mit der ID <PID>. Sie sehen die PID als Spalte im Aktivitätsmonitor
`ps -ax | grep <Anwendungsname>` Einen Prozess nach Name oder PID suchen
Netzwerk
`ping <host> `Host anpingen und Status anzeigen
`whois <Domäne>` Whois-Informationen für eine Domäne ausgeben
`curl -O <url/to/file>` Datei über HTTP, HTTPS oder FTP herunterladen
`ssh <Benutzername>@<host>` SSH-Verbindung zu <host> mit Benutzer <Benutzername> herstellen
`scp <Datei><Benutzer>@<Host>:/remote/path` Kopieren von <Datei> auf einen entfernten <Host>
`arp -a` Zeigt eine Liste aller Geräte in deinem lokalen Netzwerk an. Es zeigt Ihnen die IP- und MAC-Adresse aller Geräte an
`ifconfig en0` Anzeige der IP- und MAC-Adresse Ihres Geräts
traceroute [hostname] Identifizieren Sie den Pfad und die Hops, die die Pakete von Ihrem Gerät zur Zieladresse durchlaufen

---

####Umgebungsvariable oder Pfad
`printenv` Zeigt eine Liste der aktuell gesetzten Umgebungsvariablen an. Zeigt Ihnen auch an, welche Shell Sie benutzen
`$echo` Weist das Terminal an, etwas zu drucken und Ihnen zu zeigen
`echo PATH` Überprüft den Wert der PATH-Variablen, die eine Liste von Verzeichnissen mit ausführbaren Dateien speichert
`echo PATH >path.txt` Exportiere das Pfadverzeichnis in eine Textdatei
`export PATH=PATH:absolute/path to/program/` Führen Sie ein Programm über das Terminal nur in Ihrer aktuellen Sitzung aus. Wenn Sie ein Programm regelmäßig benutzen, fügen Sie den Pfad zur Shell-Konfigurationsdatei hinzu.

---

####Suche
`find <ordner> -name <"file">` Finde alle Dateien mit dem Namen <file> innerhalb von <ordner>. Verwenden Sie Wildcards (*), um nach Teilen von Dateinamen zu suchen
`grep "<Text>" <Datei>` Gibt alle Vorkommen von <Text> innerhalb von <Datei> aus (fügen Sie -i hinzu, um Groß- und Kleinschreibung nicht zu unterscheiden)
`grep -rl "<text>" <ordner>` Suche nach allen Dateien, die <text> innerhalb von <ordner> enthalten

####Ausgabe
`cat <Datei>` Gib den Inhalt von <Datei> aus
`less <Datei>` Den Inhalt von <Datei> mit dem less-Befehl ausgeben, der Paginierung und mehr unterstützt
head <Datei> Die ersten 10 Zeilen von <Datei> ausgeben
`< cmd> > > <file>` Hängt die Ausgabe von < cmd> an < file> an
`< cmd> > < file>` Gibt die Ausgabe von < cmd> direkt in < file> aus
`< cmd1> | < cmd2>` Lenkt die Ausgabe von < cmd1> nach < cmd2>
*die cmd commandos gehören ohne leerzeichen ins Terminal (Formatierung lässt dies hier nicht zu)*

---

####MAC Homebrew
`brew doctor` Überprüfen Sie das Gebräu auf mögliche Probleme
`brew help` Liste nützlicher Homebrew-Befehle für Formeln und Fässer
`brew install <formula>|<cask> `Installieren einer Formel oder eines Fasses
`brew uninstall <formula>|cask> `Deinstallieren einer Formel oder eines Fasses
`brew list --formula` Nur installierte Formeln auflisten
`brew list --cask` Nur installierte Fässer auflisten
`brew deps <formula>|<cask>` Alle Abhängigkeiten einer Formel oder eines Fasses auflisten
`brew search text|/regex/` Formel oder Fass über regex suchen
`brew upgrade <formula>|<cask> `Aktualisieren der Formel oder des Fasses
`brew outdated <formula>|<cask>` Suche nach veralteten Formeln oder Fässern
`brew outdated --formula` Suche nach veralteten Formeln
`brew outdated --cask` Suche nach veralteten Fässern
`brew pin [installed_formula]` Verhindern, dass eine Formel aktualisiert wird
`brew unpin [installed_formula]` Entpinnen eines Pakets zum Upgrade
`brew cleanup` Veraltete Lock-Dateien und veraltete Pakete für alle Formulare und Casks entfernen.
