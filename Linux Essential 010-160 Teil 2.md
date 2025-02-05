# Linux Essential 010-160 Teil 2

1. Welches der folgenden Verzeichnisse muss mit Lese- und Schreibzugriff gemountet werden, wenn es auf einem eigenen Dateisystem liegt?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `/var`

    Das Verzeichnis `/var` enthält variable Daten, die sich während des Betriebs des Systems ändern.
    
    </details>  

---

2. Welche Aussage über Links in einem Linux Dateisystem ist wahr?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Ein symbolischer Link kann auf eine Datei in einem anderen Dateisystem deuten

    Symbolische Links speichern nur den Pfad zum Ziel und können daher auch auf Dateien oder Verzeichnisse in anderen Dateisystemen zeigen.
    
    </details>  

---

3. Welcher Operator bei regulären Ausdrücken setzt voraus, dass das vorhergehende Zeichen null- oder einmal vorkommt?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `?`

    Der `?`-Operator sorgt dafür, dass ein Zeichen null oder einmal vorhanden sein kann. 
    
    </details>  

---

4.  Wenn man einen langen Befehl in der Shell eingibt, mit welchem Zeichen kann man den Befehl auf mehrere Zeilen aufteilen?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `\`

    Der Backslash am Ende der Zeile sorgt dafür, dass die Shell den Befehl als fortlaufend betrachtet und die Eingabe in der nächsten Zeile fortsetzt.
    
    </details>  

---

5. Welche Aussage über den Besitzer einer Datei ist wahr?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Jede Datei gehört genau einem Benutzer und einer Gruppe

    Jede Datei in einem Linux-Dateisystem hat einen Besitzer (Benutzer) und eine Gruppe. Das ist eine grundlegende Eigenschaft der Dateisystemberechtigungen.
    
    </details>  

---

6. Die meisten Befehle unter Linux können Hilfe zu ihrer Benutzung anzeigen. Wie können diese Informationen typischerweise angezeigt werden?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Indem man den Befehl mit der Option `-h` oder `--help` ausführt
    
    </details>  

---

7. Das aktuelle Verzeichnis enthält die folgenden Datei: `-rwxr-xr-x 1 root root 859688 Feb 7 08:15 test.sh`

    Angenommen die Datei ist ein gültiges Shell-Skript, wie kann dieses Skript ausgeführt werden? (Zwei auswählen)

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `bash test.sh`
    
    * `./test.sh`

    </details>  

---

8. Welche Aussagen über den `dmesg` Befehl sind wahr?

    <details>  
    <summary><b>Antwort:</b></summary>  

   * **Er zeigt den Inhalt des Linux Kernel Ring Buffers an** - Der Befehl zeigt die Meldungen aus dem Kernel-Ringpuffer an, einer Pufferzone für Kernel-Meldungen, die beim Systemstart und -betrieb generiert werden.
    
   * **Er wird möglicherweise alte Informationen nicht anzeigen, weil sie von neueren Informationen überschrieben wurden** - Der Kernel-Ringpuffer hat eine begrenzte Größe, daher können zu viele neue Nachrichten alte Informationen überschreiben.

    </details>  

---

9. Welcher der folgenden Bustypen kann Festplatten mit den Mainboard verbinden?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Der SATA-Bus

    </details>

---

10. Welcher der folgenden Werte könnte eine Prozess-ID unter Linux sein?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * 21398

    Prozess-IDs (PID) in Linux sind Ganzzahlen. Die Zahl 21398 ist ein gültiger Wert für eine PID.

    </details>

---

11. Warum werden Webbrowser-Cookies als gefährlich angesehen?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Cookies ermöglichen die Identifikation und das Tracking von Benutzern

    Cookies werden häufig verwendet, um Benutzer bei verschiedenen Besuchen zu identifizieren und ihr Verhalten zu verfolgen. Diese Daten können dann für gezielte Werbung, Analysezwecke oder sogar zum Diebstahl von Identitätsinformationen verwendet werden, was ein Datenschutzrisiko darstellt.

    </details>

---

12. Welcher der folgenden Befehle kann benutzt werden, um einen DNS Namen in eine IP-Adresse aufzulösen?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `host`

    </details>

---

13. Welches Schlüsselwort wird in einem Shell-Skript benutzt, um eine Schleife (loop) zu beginnen?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `for`

    Beispiel:

    ```bash
    #!/bin/bash

    for i in {1..5}
    do
    echo "Iteration number: $i"
    done
    ```

    </details>

---

14. Welche der folgenden Befehle sortiert die Ausgabe des Befehls `export-logs`?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `export-logs | sort`

    Der Befehl `sort` sortiert die Eingaben in alphabetisch aufsteigender Reihenfolge. Mit dem Pipe-Symbol | kann die Standardausgabe der `export-logs` durch sortieren geleitet werden.

    </details>

---

15. Welches der folgenden Zeichen in einem Shell-Prompt zeigt an, dass die Shell mit root-Rechten ausgeführt wird?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `#`

    Das `#` steht für die Root-Eingabeaufforderung, während das `$` für die Benutzer-Eingabeaufforderung steht.

    </details>

---

16. Welcher der folgenden Befehle setzt die Variable `USERNAME` auf den Wert `bob`?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `USERNAME=bob`

    In Bash wird eine Variable einfach durch Zuweisung des Werts an den Variablennamen ohne Leerzeichen gesetzt.

    </details>

---

17. Was ist die UID des Benutzers `root`?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * 0

    Laut `/etc/passwd`:

    `root:x:0:0:Super User:/root:/bin/bash`

    Beachten Sie die 0 für UID und 0 für GID.

    </details>

---

18. Welche der folgenden Aussagen über Freie Software ist wahr?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Kann von jedem, der sie benutzt, verändert werden

    Der Begriff "freie Software" bezieht sich auf die Freiheit der Nutzer, die Software zu verwenden, zu verändern und weiterzugeben. Eine der vier grundlegenden Freiheiten der freien Software ist die Freiheit, den Quellcode zu verändern.

    </details>

---

19. Der Besitzer der Datei `doku.odt` soll geändert werden. Der neue Besitzer heißt `tux`.

    Welcher Befehl erfüllt diese Aufgabe?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `chown tux doku.odt`

    `chown` benötigt zuerst den Benutzernamen des neuen Besitzers und dann den Namen der Datei, die geändert werden soll.

    </details>

---

20. Welches der folgenden Programme sind Webserver?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * NGINX
    
    * Apache HTTPD

    </details>

---

21. Welches der folgenden Beispiele zeigt die allgemeine Struktur einer for-Schleife in einem Shell-Skript?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `for i in *.txt do echo $i done`

    ```bash
    for VARIABLE in LISTE
    do
      BEFEHLE
    done
    ```

    Die Schleife geht durch alle Dateien mit der Erweiterung `.txt` und gibt deren Namen aus.


    </details>

---

22. Wo ist das Betriebsystem bei einem Raspberry Pi gespeichert?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Auf einer wechselbaren SD-Karte, die in den Pi gesteckt wird

    </details>

---

23. Welche der folgenden Ausgaben stammt vom Befehl `free`?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Option E

    ```
                   total        used        free      shared  buff/cache   available
    Mem:         3948900     1661528     1063584       16636     1488320     2287372
    Swap:        3948540           0     3948540
    ```

    `free` zeigt die Menge des freien und verwendeten Arbeitsspeichers im System an.

    </details>

---

24. Welche der folgenden Aufgaben kann der Befehl `passwd` erfüllen?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * **Das Passwort eines Benutzers ändern** - Wenn der Befehl ohne weitere Optionen ausgeführt wird, ändert er das Passwort des aktuellen Benutzers.

    * **Ein Benutzerkonto sperren** - Die Option `-l` sperrt das Konto und verhindert, dass sich der Benutzer anmeldet.

    </details>

---

25. Welche der folgenden Befehle werden benutzt, um Informationen über die richtige Verwendung von `ls` zu bekommen?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `man ls`

    * `info ls`

    </details>

---

26. Welcher der folgenden Befehle findet alle Zeilen in der Datei `operating-systems.txt`, die den Begriff `linux` enthalten, egal ob groß oder kleingeschrieben?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `grep -i linux operating-systems.txt`

    `grep` sucht mit Hilfe von Regex nach Mustern in Dateien. Die Option `-i` gibt an, dass die Groß-/Kleinschreibung ignoriert wird.

    </details>

---

27. Was findet sich im `/proc/` Verzeichnis?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Ein Verzeichnis für jeden laufenden Prozess

    Das `/proc`-Dateisystem dient als Schnittstelle zu Kernel-Datenstrukturen und Laufzeitinformationen

    </details>

---

28. Was passiert mit einer Datei außerhalb des Home-Verzeichnisses, wenn das Benutzerkonto, dem die Datei gehört, gelöscht wird?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Die UID des vorherigen Besitzers wird angezeigt, wenn man die Details der Datei anschaut

    * Besitzer und Berechtigungen der Datei bleiben unverändert 

    </details>

---

29. Welches der folgenden ist ein Protokoll, das für die automatische IP Adresskonfiguration benutzt wird?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * DHCP

    </details>

---

30. Ein neuer Server muss installiert werden, um Dienste für einen Zeitraum von mehreren Jahren zu hosten. Während dieser Zeit muss der Server wichtige Sicherheitsupdates von seiner Linux-Distribution erhalten.

    Welche der folgenden Linux-Distributionen erfüllt diese Anforderung?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * **Ubuntu Linux LTS** - bietet langjährige Unterstützung (fünf Jahre für Desktop und Server) und regelmäßige Sicherheitsupdates.

    * **Red Hat Enterprise Linux** - bietet langjährige Unterstützung mit regelmäßigen Sicherheitsupdates

    </details>

---

31. Welche der folgenden Aussagen über Linux Passwörter ist wahr?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Passwörter werden nur in Hash-Form gespeichert

    Die gehashten Passwörter werden in `/etc/shadow` gespeichert

    </details>

---

32. Ein Verzeichnis enthält die folgenden drei Dateien:

    ```
    texts 1.txt
    texts 2.txt
    texts 3.csv
    ```

    Welcher Befehl kopiert die beiden Dateien, die auf `.txt` enden, in das `/tmp/` Verzeichnis?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `cp *.txt /tmp/`

    </details>

---

33. Aus welchen Dateien werden die Informationen für die folgende Ausgabe entnommen:
    
    `uid=1000 (bob) gid=1000 (bob) groups=1000 (bob), 10 (wheel), 150 (docker), 989 (wireshark), 1001 (libvirt)`

    <details>  
    <summary><b>Antwort:</b></summary>  

    * `/etc/group` -  Die Datei enthält Informationen zu den Gruppen eines Systems, einschließlich der Gruppennamen und der Gruppen-IDs (GID).

    * `/etc/passwd` - Die Datei enthält Benutzerinformationen, einschließlich der Benutzer-IDs (UID) und Gruppen-IDs (GID).

    </details>

---

34. Welche Informationen können von `top` angezeigt werden?

    <details>  
    <summary><b>Antwort:</b></summary>  

    * Laufende Prozesse, sortiert nach CPU- oder RAM-Verbrauch

    `top` ist ein Echtzeit-Systemmonitor, der Informationen zu laufenden Prozessen anzeigt.

    </details>

---