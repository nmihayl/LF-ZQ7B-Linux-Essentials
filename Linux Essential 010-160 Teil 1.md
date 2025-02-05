# Linux Essential 010-160  

1. Welche Informationen sind in der Datei `/etc/passwd` gespeichert?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Benutzername  
    * Numerische Benutzer-ID  
    * Die Standard-Shell des Benutzers  

    Beispiel für einen Eintrag in `/etc/passwd`:  

    ```plaintext
    nick:x:1000:1000:nick:/home/nick:/bin/zsh
    ```

    Aufbau der Einträge:  

    ```plaintext
    [username]  [password]  [UID]   [GID]   [GECOS] [home]  [shell]
    ```
    </details>  

---

1. Die Datei `script.sh` im aktuellen Verzeichnis hat den folgenden Inhalt:

    ```bash
    #!/bin/bash
    echo $MYVAR
    ```  

    Das folgende Kommando wird benutzt, um dieses Skript auszuführen:

    ```bash
    MYVAR=value
    ./script.sh
    ```  

    Das Ergebnis ist eine leere Zeile, anstatt des Inhalts der Variablen `MYVAR`.

    Wie sollte `MYVAR` stattdessen gesetzt werden, damit das Skript den Inhalt von `MYVAR` ausgibt?

    <details>  
    <summary><b>Antwort:</b></summary>  

    ```bash
    export MYVAR=value
    ```  
    </details>  

---

3. Beim Ausführen des Befehls `rm Downloads` erscheint folgende Fehlermeldung: `rm: cannot remove 'Downloads/': Is a directory`
   
   Welcher der folgenden Befehle kann stattdessen benutzt werden, um Downloads zu löschen, vorausgesetzt Downloads ist leer?

   <details>  
    <summary><b>Antwort:</b></summary>  

    * `rm -r Downloads` (Rekursives Löschen aller Inhalte innerhalb eines Verzeichnisses) 

    * `rmdir Downloads` (Funktioniert nur mit leeren Verzeichnissen)

    </details>  

---

4. Ein Benutzer ist gerade im Verzeichnis `/home/user/Downloads/` und führt den Befehl `ls ../Documents/` aus.
    
    Der Inhalt welches Verzeichnisses wird angezeigt, vorausgesetzt es existiert?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `/home/user/Documents`
  
    Der `..` steht für das oberste Verzeichnis im relativen Verzeichnisbaum.

    </details>  

---

5. Welcher Befehl zeigt Manual Pages an? (nur den Befehl ohne Pfad oder Parameter eingeben)
   
   <details>  
    <summary><b>Antwort:</b></summary>  

    * `man`

    Pfad:

    `/usr/bin/man`

    </details>  

---

6. Welches der folgenden Programme ist ein grafisches Bearbeitungsprogramm für Vektorgrafiken?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Inkscape

    </details>  

---

7. Was ist der Rückgabewert eines Shell-Skripts nach erfolgreicher Ausführung?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `0`

    Exit codes:

    `0` = Erfolg

    `1` = Fehler (generell)

    `255` = Abnormale Beendigung eines Prozesses

    `-1` = ungültig in Bash

    `-255` = ungültig in Bash

    </details>  

---

8. Was ist die bevorzugte Quelle für die Installation neuer Anwendungsprogramme in einem Linux-basierten Betriebsystem?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Das Paket-Repository der Distribution

    </details>  

---

9. Welcher der folgenden Befehle gibt den Inhalt der Datei `Texts 2.txt` aus?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `cat Texts\ 2.txt`

    * `cat 'Texts 2.txt'`

    Mit `\ ` kann man ein Leerzeichen definieren, das erforderlich ist, wenn der Dateiname eines hat, sonst wird es als mehrere Parameter interpretiert.

    Wenn ein Dateiname in Anführungszeichen steht, kann das Leerzeichen hinzugefügt werden, da es den Befehl nicht beeinträchtigt. Ein `\ ` in Anführungszeichen ist jedoch ungültig und wird als Teil des Dateinamens wahrgenommen.

    </details>  

---

10. Welches der folgenden Geräte repräsentiert eine Festplatten-Partition

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `/dev/sda2`

    Unter Linux stellt `/dev/sd*` ein Blockgerät dar, wobei jedes numerische Suffix die Partition des Blockgeräts darstellt.

    </details>  

---

11. Welcher Befehl erstellt den neuen Benutzer `tux` und erstellt sein Homeverzeichnis mit den default Konfigurationsdateien?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `useradd -m tux`

    Das Flag `-m` ist wichtig, wenn Sie einen neuen Benutzer mit einem Home-Verzeichnis unter `/home` erstellen.

    </details>  

---

12. Welcher der folgenden Befehle erstellt das Zip-Archiv `poems.zip` mit allen Dateien aus dem aktuellen Verzeichnis, deren Namen auf `.txt` enden?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `zip poems.zip *.txt`

    Der Befehl `zip` verlangt zunächst den Namen der Ausgabedatei `poems.zip` und dann die Angabe des Archivinhalts mit dem Platzhalter `*.txt`

    </details>  

---

13. Welches Paketverwaltungs-Tool wird in Red-Hat basierten Linux Systemen verwendet?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `rpm`

    </details>  

---

14. Welche Aussage über den `su` Befehl ist wahr?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Er führt eine Shell oder Befehle als anderer Benutzer aus

    Wenn Sie `su` ohne Optionen oder Flags verwenden, wird standardmäßig die Root-Login-Shell verwendet.

    </details>  

---

15. Welcher der folgenden Befehle sucht nach der Datei `foo.txt` im Verzeichnis `/home`?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `find /home -name foo.txt`

    Beim `find`-Befehl wird zunächst das Verzeichnis benötigt, in dem gesucht werden soll, anschließend kann mit `-name` der gewünschte Dateiname übergeben werden.

    </details> 

---

16. Welche der folgenden `tar`-Optionen ermöglicht die Komprimierung?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `-z` (Verwendet gzip-Komprimierung)

    * `-j` (Verwendet bzip2-Komprimierung)

    </details> 

---

17. Welcher der folgenden Befehle extrahiert den Inhalt aus dem komprimierten Archiv file1.tar.gz?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `tar -xzf file1.tar.gz`

    Mit `-x` wird eine Extraktion des Archivs eingeleitet, das Flag `-z` gibt den Typ des zu extrahierenden Archivs an (in diesem Fall gzip) und `-f` wird verwendet, um die Eingabearchivdatei anzugeben.

    </details> 

---

18. Die Mitglieder eines Teams haben bereits Erfahrung mit Red Hat Enterpise Linux. Für ein kleines Hobbyprojekt will das Team einen Linux-Server aufsetzen, ohne für ein Support-Abonnement bezahlen zu müssen. Welche der folgenden Distributionen ermöglicht den Teammitgliedern, möglichst viel von ihrer Red Hat Enterprise Linux-Erfahrung bei dem Projekt anwenden zu können?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * CentOS

    </details> 

---

19. Was wird durch eine Softwarelizenz definiert?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Bedingungen für das Modifizieren und Weiterverbreiten der Software

    </details> 

---

20. Welches der folgenden Verzeichnisse enthält Informationen, Dokumentation und Beispiel-Konfigurationsdateien für installierte Softwarepakete?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `/usr/share/doc/`

    </details> 