# LF-ZQ7B Linux Essentials

## 1.1

**1. Inwiefern unterscheidet sich Debian GNU/Linux von Ubuntu? Nennen Sie zwei Aspekte.**

- Debian ist eine von der Community entwickelte Distribution, während Ubuntu von der Firma Canonical entwickelt wird.

- Debian konzentriert sich auf die Bereitstellung gründlich getesteter stabiler Software, während Ubuntu neuere, wenn auch etwas instabilere Softwarepakete bereitstellen kann.

**2. Welche sind die gängigsten Umgebungen/Plattformen, in denen Linux eingesetzt wird? Nennen Sie drei verschiedene Umgebungen/Plattformen und nennen Sie eine Distribution, die sich für alle eignet.**

- Server (Debian)

- Desktop (Ubuntu)

- Smartphone (Android)

**3. Welche sind die gängigsten Umgebungen/Plattformen, in denen Linux eingesetzt wird? Nennen Sie drei verschiedene Umgebungen/Plattformen und nennen Sie eine Distribution, die sich für alle eignet.**

- Lizenzierung

- Kosten

- Hardware-Support

- Stabilität

**4. Nennen Sie — abgesehen von Smartphones — drei Geräte, auf denen das Android-Betriebssystem läuft.**

- Smart TVs

- Android Auto

- Smartwatches

**5. Erklären Sie drei wesentliche Vorteile von Cloud Computing.**

- Skalierbarkeit

- Kosteneffizienz

- Verfügbarkeit

## 1.1 (offene)

**1. Welche Distributionen sind in Bezug auf Kosten und Leistung am besten für ein Unternehmen geeignet, das darauf abzielt, die Lizenzkosten zu senken und gleichzeitig die Leistung auf dem höchsten Niveau zu halten? Erklären Sie, warum.**

- **Debian**: kostenlos und priorisiert Stabilität auf Kosten der Paketaktualität.

- **Fedora**: kostenlos, dient als Upstream für RHEL und bietet gleichzeitig neuere Pakete und sofort einsatzbereite Unterstützung für SELinux

- **Ubuntu**: kostenlos mit kommerzieller Unterstützung durch viele Unternehmen, was Stabilität für den Einsatz in Unternehmen gewährleistet

**2. Was sind die Hauptvorteile des Raspberry Pi und welche Funktionen kann er in Unternehmen erfüllen?**

- **Preis-Leistungs-Verhältnis**: Der Raspberry Pi kann für die Leistung, die er bietet, relativ erschwinglich sein (abhängig von der Hardwarekonfiguration).

- **Effizienz**: Da es sich um eine ARM-basierte Plattform handelt, kann er mit relativ geringem Energieverbrauch arbeiten, was eine effiziente Leistungsaufnahme gewährleistet.

- **Portabilität und Größe**: Der geringe Platzbedarf des Raspberry Pi macht ihn zu einem idealen Thin Client.

**3. Welche Distributionen bieten Amazon Cloud Services und Google Cloud an? Nennen Sie mindestens drei gemeinsame und zwei verschiedene.**

**Auf beiden Plattformen verfügbar**: Debian, RHEL, CentOS

**Einzigartig für beide Plattformen**: Amazon Linux, Rocky Linux (Google Cloud Services)

## 1.2

**1. Identifizieren Sie für jeden der folgenden Befehle, ob er zum Debian-Paketverwaltungssystem oder zum Red Hat-Paketverwaltungssystem gehört:**

| Paketmanager | Distribution                  |
| ------------ | ----------------------------- |
| `dpkg`       | Debian                        |
| `rpm`        | Red Hat                       |
| `apt-get`    | Debian (Standard auf Ubuntu)  |
| `yum`        | Red Hat                       |
| `dnf`        | Red Hat (Standard auf Fedora) |

**2. Welcher Befehl könnte verwendet werden, um Blender auf Ubuntu zu installieren? Wie kann das Programm nach der Installation ausgeführt werden?**

`apt install blender -y`

Das Programm kann entweder über die Befehlszeile mit `blender` oder über den grafischen Anwendungsstarter in der Desktopumgebung ausgeführt werden.

**3. Welche Anwendung aus der LibreOffice Suite dient der elektronischen Tabellenkalkulation?**

LibreOffice Calc (`libreoffice --calc`).

**4. Welcher Open-Source-Webbrowser bildet die Grundlage für die Entwicklung von Google Chrome?**

Chromium (`chromium`).

**5. SVG ist ein offener Standard für Vektorgrafiken. Welche ist die beliebteste Anwendung zum Bearbeiten von SVG-Dateien in Linux-Systemen?**

Inkscape (`inkscape`).

**6. Schreiben Sie für jedes der folgenden Dateiformate den Namen einer Anwendung, die die entsprechende Datei öffnen und bearbeiten kann:**

| Extension | Anwendung                                   |
| --------- | ------------------------------------------- |
| `png`     | GIMP, ImageMagick, Krita, mpv               |
| `doc`     | LibreOffice Writer, OpenOffice, ONLYOFFICE  |
| `xls`     | LibreOffice Calc, OpenOffice, ONLYOFFICE    |
| `ppt`     | LibreOffice Impress, OpenOffice, ONLYOFFICE |
| `wav`     | ffmpeg, Audacity, mpv, Audacious            |

**7. Welches Softwarepaket ermöglicht den Dateiaustausch zwischen Linux- und Windows-Rechnern über das lokale Netzwerk?**

Samba (`samba` für Serveranwendung, `smbclient` für Clientanwendung)

**8. Sie wissen, dass Konfigurationsdateien auch dann erhalten bleiben, wenn das zugehörige Paket aus dem System entfernt wird. Wie können Sie das Paket namens cups und seine Konfigurationsdateien automatisch aus einem DEB-basierten System entfernen?**

`apt purge cups`

**9. Angenommen Sie haben viele TIFF-Bilddateien und mochten diese in JPEG konvertieren. Welches Softwarepaket konnte verwendet werden, um diese Dateien direkt auf der Kommandozeile zu konvertieren?**

`apt install imagemagick -y`

`magick eingabe.tiff ausgabe.jpg`

**10. Welches Softwarepaket müssen Sie installieren, um Microsoft-Word-Dokumente öffnen zu können, die Ihnen von einem Windows-Benutzer zugesandt wurden?**

`apt install libreoffice`

## 1.3

**1. Wie lauten — in Kurzfrom — die “vier Freiheiten”, wie sie von Richard Stallman und der Free Software Foundation definiert wurden?**

| Freiheit | Beschreibung                                                                                                                                                                                                                                         |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0        | Die Freiheit, das Programm nach Belieben und zu jedem Zweck auszuführen.                                                                                                                                                                             |
| 1        | Die Freiheit, die Funktionsweise des Programms zu untersuchen und es so zu ändern, dass es Ihre Rechenaufgaben nach Ihren Wünschen erledigt. Der Zugriff auf den Quellcode ist hierfür eine Voraussetzung.                                           |
| 2        | Die Freiheit, Kopien weiterzugeben, damit Sie Ihrem Nachbarn helfen können.                                                                                                                                                                          |
| 3        | Die Freiheit, Kopien Ihrer geänderten Versionen an andere weiterzugeben. Auf diese Weise können Sie der gesamten Community die Möglichkeit geben, von Ihren Änderungen zu profitieren. Der Zugriff auf den Quellcode ist hierfür eine Voraussetzung. |

**2. Wofür steht die Abkürzung FLOSS?**

**F**ree **L**ibre **O**pen **S**ource **So**ftware

**3. Sie haben Software entwickelt und möchten sicherstellen, dass die Software selbst, aber auch alle künftigen darauf aufbauenden Ergebnisse ebenso frei bleiben. Welche Lizenz wählen Sie?**

GNU General Public License v3.0 (GNU GPLv3)

**4. Welche der folgenden Lizenzen würde man als permissive bezeichnen, welche als Copyleft?**

| Lizenz                 | Art        |
| ---------------------- | ---------- |
| Simplified BSD License | Permissive |
| GPL v3                 | Copyleft   |
| CC BY                  | Permissive |
| CC BY-SA               | Copyleft   |

**5. Sie haben eine Webapplikation geschrieben und unter einer freien Lizenz veröffentlicht. Wie können Sie mit Ihrem Produkt Geld verdienen? Nennen Sie drei Möglichkeiten.**

- Premium-Support anbieten

- Gebühren für die Anwendung erheben und gleichzeitig den Quellcode verfügbar halten (dies ist unter der GNU GPL möglich)

- Den Quellcode für die Basisanwendung verfügbar halten, aber für alle zusätzlichen Extras Gebühren erheben

**6. Unter welcher Lizenz (einschließlich Version) stehen die folgenden Anwendungen?**

| Anwendung              | Lizenz                     |
| ---------------------- | -------------------------- |
| Apache HTTP Server     | Apache License             |
| MySQL Community Server | GNU General Public License |
| Wikipedia Artikel      | CC BY-SA                   |
| Mozilla Firefox        | Mozilla Public License     |
| GIMP                   | GNU General Public License |

**7. Sie mochten Ihre Software unter der GNU GPL v3 veröffentlichen. Welche Schritte sollten Sie beachten?**

| Berechtigungen       | Bedingungen                      | Einschränkungen |
| -------------------- | -------------------------------- | --------------- |
| Kommerzielle Nutzung | Quellcode offenlegen             | Haftung         |
| Verbreitung          | Lizenz- und Urheberrechtshinweis | Garantie        |
| Modifikation         | Gleiche Lizenz                   |                 |
| Patentnutzung        | Änderungen angeben               |                 |
| Private Nutzung      |                                  |                 |

**8. Sie haben proprietäre Software geschrieben und würden sie gerne mit freier Software unter der GPL v3 kombinieren. Dürfen Sie das bzw. was müssen Sie beachten?**

- **Copyleft-Bedingung**: Wenn GPLv3-Software mit proprietärer Software kombiniert und verteilt wird, muss das gesamte Werk unter der GPLv3 stehen.

- **Veröffentlichung des Quellcodes**: Der gesamte Quellcode muss offengelegt werden, einschließlich des proprietären Codes, und muss unter der GPL v3 lizenziert sein.

**9. Warum hat die Free Software Foundation als Ergänzung zur GNU GPL die GNU Affero General Public License 3 (GNU AGPL) veröffentlicht?**

Die AGPL ist in erster Linie für Webanwendungen gedacht und erweitert die GPL um die Nutzung über ein Netzwerk. Sie enthält eine zusätzliche Bedingung, die es Benutzern, die über ein Netzwerk mit der lizenzierten Software interagieren, ermöglicht, den Quellcode für dieses Programm zu erhalten.

**10. Nennen Sie drei Beispiele freier Software, die auch als „Business Edition“ , also in einer kostenpflichtigen Version angeboten werden.**

- Red Hat Enterprise Linux (RHEL)

- GitLab

- MySQL