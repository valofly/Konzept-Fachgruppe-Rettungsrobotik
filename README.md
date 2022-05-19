# Einsatz- und Ausbildungskonzept "Rettungsrobotik"
Das vorliegende Konzept ist für Behörden und Organisationen gedacht, welche eine Fachgruppe Rettungsrobotik, eine Drohnengruppe oder Drohnenstaffel umsetzen wollen oder müssen. Das Konzept arbeitet am Beispiel der Feuerwehr, lässt sich jedoch auch auf das Technische Hilfswerk oder Rettungsdienste umschreiben.

Bitte gebt eure Änderungen und Anmerkungen oder sogar die eigene Version eures Konzeptes an die Gemeinschaft zurück, damit alle etwas davon haben.

## Erstellen der PDF
Das vorliegende Konzept ist in LaTeX geschrieben, um plattformunabhängig von allen genutzt werden zu können. Um das Dokument zu generieren, wird das LaTeX-Softwarepacket und ein entsprechender Editor (jeweils kostenfrei) benötigt.

### Installation LaTeX
Linux: https://tug.org/texlive/quickinstall.html aufrufen und der Anleitung unter *Running the installer* folgen.
Windows: https://tug.org/texlive/windows.html aufrufen, install-tl-windows.exe herunterladen und installieren.
MacOS: https://tug.org/mactex/ aufrufen, das MacTeX-Paket herunterladen und installieren.

### Installation Editor
Es gibt verschiedene Editoren zum Bearbeiten von .tex Dateien, die frei gewählt werden können. Einer davon ist TexMaker. Dieser kann unter https://www.xm1math.net/texmaker/ für Linux, Windows und MacOS heruntergeladen werden.

### Ausbildungskonzept herunterladen
Über den grünen Button `Code` könnt mittels Git-Client die Dateien clonen. Für Personen, die erstmalig mit GitHub in Berührung kommen, empfiehlt sich `Download ZIP`.

### PDF generieren
Um das PDF zu generieren, muss die Datei `concept_RettR.tex` mit dem LaTeX-Editor geöffnet und kompiliert werden. In TexMaker erfolgt dies über "Schnelles Übersetzen". In dem Ordner, der die `concept_RettR.tex` enthält, werden nun Hilfsdateien und das fertige PDF `concept_RettR.pdf` erzeugt.

**Hinweis:** Teilweise muss das Dokument zweimal erstellt werden, um alle Querverweise zu setzen. Ob dies notwendig ist, kann z. B. am Fehlen des Inhaltsverzeichnisses erkannt werden.

## Konzept auf eure Einheit anpassen (einfach)
Zum Anpassen auf eure Einheit muss die Datei `definitions.tex` verändert werden. Diese enthält Variablen, die das Dokument auf euch anpassen. Nach der Anpassung der Variablen kann `concept_RettR.tex` neu erstellt werden. Das PDF enthält automatisch eure Anpassungen.

| Variable | Parameter | Beschreibung / Anmerkung
|--|--|--|
| `docVersion` | YYYYMMDD | die Version des Dokumentes. Diese wird in hellgrau am linken Rand angezeigt. |
| `dmoGroup` | DMO Rufgruppe | Die vorgehaltene Rufgruppe zum Betrieb von UAV, UGV, UUV. |
| `district` | Name des Landkreises | Das Konzept ist auf Landkreisebene angepasst. Für Städte und Gemeinden sind einige Änderungen notwendig. |
| `state` | Bundesland | Angabe des Bundeslandes. |
| `unit` | Übergeordnete Einheit | Das Konzept geht davon aus, dass es übergeordnete Einheiten gibt. Andernfalls sind einige Änderungen notwendig. |
| `platoon` | Zug innerhalb von `unit` | Das Konzept geht davon aus, dass die Gruppe in einen Zug eingebunden ist. Andernfalls sind einige Änderungen notwendig. |
| `specialistGroup` | Name der Einheit | Dieser kann auf "Rettungsrobotik", "Drohnengruppe", "Drohnenstaffel", […] lauten. |
| `gruppenfuehrer` | Name für Gruppenführer | Entspr. FwDV 3, Angepasste Benennung für den Gruppenführer. |
| `melder` | Name für Melder | Entspr. FwDV 3, Angepasste Benennung für den Melder. Z. B. Koordinator Robotik, Flugleiter, … |
| `maschinist` | Name für Maschinist | Entspr. FwDV 3, Angepasste Benennung für den Maschinist. Z. B. "Informationsauswerter", "Bildauswerter", … |
| `angriffstrupp` | Name für Angriffstrupp | Entspr. FwDV 3, Angepasste Benennung für den Angriffstrupp. |
| `wassertrupp` | Name für Wassertrupp | Entspr. FwDV 3, Angepasste Benennung für den Wassertrupp. |
| `schlauchtrupp` | Name für Schlauchtrupp | Entspr. FwDV 3, Angepasste Benennung für den Schlauchtrupp. |
| `robotiktrupp` | Name innerhalb `angriffstrupp` und `wassertrupp` | Variable um Benennung von Angriffs- und Wassertrupp identisch zu halten.  |
| `operatorName` | UAS-Betreiber Name | Name des UAS-Betreibers |
| `operatorStreet` | UAS-Betreiber Straße | Adresse des UAS-Betreibers |
| `operatorZIP` | UAS-Betreiber Postleitzahl | Adresse des UAS-Betreibers |
| `operatorCity` | UAS-Betreiber Stadt | Adresse des UAS-Betreibers |
| `operatorID` | UAS-Betreiber ID | Durch LBA zugewiesene UAS-Betreiber ID |
| `callee` | Name für generischen Begriff "Einheit" im Text. | Im Textfluss wird dann von "Einheit", "Fachgruppe", "Drohneneinheit", … gesprochen. |
| `FwDVI` | FwDV 1 | Link auf die Feuerwehrdienstvorschrift 1 entsprechend des Bundeslandes |
| `FwDVIII` | FwDV 3 | Link auf die Feuerwehrdienstvorschrift 3 entsprechend des Bundeslandes |
| `FwDVC` | FwDV 100 | Link auf die Feuerwehrdienstvorschrift 100 entsprechend des Bundeslandes |
| `FwDVD` | FwDV 500 | Link auf die Feuerwehrdienstvorschrift 500 entsprechend des Bundeslandes |
| `FwDDCCC` | FwDV 800 | Link auf die Feuerwehrdienstvorschrift 800 entsprechend des Bundeslandes |
| `FwDDCCCX` | FwDV 810 | Link auf die Feuerwehrdienstvorschrift 810 entsprechend des Bundeslandes |

Das Wappen eures Landkreises müsst ihr als `logo_Landkreis` in einem der unterstützen Formate im Ordner `images` ablegen. LaTeX unterstützt nativ nur die Bildformate `PS`, `EPS`, `PDF`, `GIF`, `JPG`, und `TIF`.

TODO Derzeit funktionieren nur Logos im `PDF` Format. Wird noch angepasst.

## Konzept auf eure Einheit anpassen (komplex)
Das Dokument besteht im Wesentlichen aus der `concept_RettR.tex` sowie den Dateien für die einzelnen Kapitel. Diese sind im Ordner `chapter` abgelegt. In den einzelnen Kapiteln

 1. `chapter`/`01_basics` (Grundlagen)
 2. `chapter`/`02_purpose` (Aufgaben)
 3. `chapter`/`03_organization` (Aufbau und Gliederung)
 4. `chapter`/`04_alerting` (Alarmierung)
 5. `chapter`/`05_equipment` (Ausrüstung)
 6. `chapter`/`06_training` (Ausbildung)
 7. `chapter`/`07_documentation` (Dokumentation)
 8. `chapter`/`08_miscellaneous` (Sonstiges)

findet ihr die Inhalte des Konzeptes. Sollen nun Inhalte umgeschrieben, hinzugefügt oder gelöscht werden, kann dies einfach in den Dateien erfolgen. Nach dem Anpassen muss das Dokument zur besseren Lesbarkeit wieder als PDF erzeugt werden.

**Hinweis:** Zum erneuten Erzeugen muss das bereits erzeugte PDF geschlossen sein, da dieses überschrieben wird.

Die Dateien `abbreviation_list.tex`, `packages.tex` und `titlepage.tex` enthalten i. d. R. das Abkürzungsverzeichnis, die benötigten Pakete zum Erstellen des Dokumentes sowie die Titelseite. Ändert diese Dateien, insbesondere die `packages.tex` nur, wenn ihr euch auskennt.

## Änderungen und Verbesserungen
Es gibt mehrere Möglichkeiten an der Verbesserung des Konzeptes mitzuwirken.

### Issue erstellen
Ihr könnt über https://github.com/valofly/Konzept-Fachgruppe-Rettungsrobotik/issues eine Anmerkung erstellen. Hierzu wird ein GitHub-Account benötigt.

Die Anmerkung kann anschließend von allen Interessierten direkt am Projekt diskutiert werden. Wichtig: Sachlich bleiben.

### Aktiv mitwirken
Änderungen können direkt erstellt und eingereicht werden. Nach einer Prüfung und (evtl.) Diskussion kann eine Änderung direkt in das Projekt zurückfließen, sodass alle davon profitieren.

## Vorschau zum Konzept
Das Konzept kann unter https://acrobat.adobe.com/link/review?uri=urn:aaid:scds:US:1cf34671-1c3f-365d-9ab3-e3df6bd66aea eingesehen werden. Kommentare sind möglich, werden jedoch nicht überwacht.
