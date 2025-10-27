# Abschlussprojekt DBE-Academy Frontend Web Developer
### Projekt: **Stechen**-Helper
### Inhaltsverzeichnis
1. [Einleitung](#einleitung)
2. [Projektbeschreibung](#projektbeschreibung)
3. [Technische Anforderungen](#technische-anforderungen)

## Einleitung
Das **Stechen**-Helper Projekt ist eine Webanwendung, die entwickelt wird, um die Organisation und Verwaltung von dem Kartenspiel "**Stechen**" zu erleichtern. Die Anwendung soll Benutzern helfen, **Stechen**-Partien zu planen, zu verwalten und zu verfolgen, indem sie eine benutzerfreundliche Oberfläche und leistungsstarke Funktionen bietet. Diese Webanwendung wird für **Tablets und Desktop** entwickelt, aber geeignete, große Handys im Querformat werden ebenfalls unterstützt.

## Projektbeschreibung
### Die Idee
Das Kartenspiel **Stechen** ist in meiner Familie ein beliebtes Gesellschaftsspiel, das oft mit Freunden und der Familie gespielt wird. Es basiert auf dem Kartenspiel [**11er Raus**](https://amzn.eu/d/eReStgf), dessen Regeln ich gleich noch näher erläutere. Für dieses Spiel braucht man einen Schriftführer, der die Punkte mitschreibt und so später dann der Gewinner ermittelt werden kann. Und HIER kommt die App ins Spiel. Meine App soll den Papieraufwand minimieren, wenn nicht gleich eliminieren und einen schnelleren und zugleich komplett regelkonformen Ablauf zu gewährleisten. Das *tracken* einer Partie ist aber nur ein Teil der App. Mit dieser App soll man zudem auch mehrere Spielgruppen organisieren können und Ranglisten sowie Spielerstärken ermitteln.

### Die Regeln des Spiels **Stechen**
Für dieses Spiel benötigt man das oben erwähnte **11er Raus** Kartenspiel. **Stechen** ist ein Spiel für min. 2 und maximal 11 Personen. Den meisten Spielspaß hat man allerdings erst ab mindestens drei Personen.

Ziel dieses Spieles ist es, durch geschicktes Analysieren seiner Karten und ansagen seiner zu erwartenden Stiche eine bestimmte Punktzahl als erstes so schnell wie möglich zu erreichen.

Das **11er Raus** Kartenspiel besteht aus 80 Karten, aufgeteilt in 4 Farben, rot, gelb, grün und blau, zu Werten von 1-20. Daher ergibt sich auch die Höchstgrenze für Mitspieler: 11 Spieler á 7 Karten = 77 Karten, drei rest im Stack. Davon eine Karte noch als Trumpf-Karte = 78 Karten, zwei verbleibend.

Je nach Anzahl der Spieler gibt es unterschiedliche Anzahl von Karten, die die Spieler zu Beginn erhalten:
- 2 - 6 Spieler: 9 Karten
- 7 - 11 Spieler: 7 Karten

Die restlichen Karten verbleiben als Stapel, wobei noch EINE Karte als Trumpfkarte/Trumpf-Farbe aufgedeckt auf den Stapel gelegt wird.

Zu Beginn des Spieles wird der Kartengeber (Dealer) bestimmt, danach wechselt dieser pro Spielrunde im Uhrzeigersinn. Der Dealer mischt die Karten und teilt sie aus. Danach wird die Trumpfkarte aufgedeckt. Eine Runde besteht aus drei Spielabschnitten, die nun näher erläutert werden.
#### Das Ansagen
In diesem Spielabschnitt startet der Spieler **links vom Dealer** mit den Ansagen. Einen sogenannten *Stich* kann man machen, wenn man mit der ausgespielten Farbe die Höchste Zahl selbst hat oder, wenn die ausgespielte Karte keine Trumpf-Farbe ist, die höchste Trumpf-Farbenkarte auf den Tisch legt. Entscheidend ist, dass man die Farbe, die ausgespielt wurde, bedienen muss, es sei denn, man hat diese Farbe nicht. Dann kann man entweder eine Trumpf-Farbe legen und so eventuell den Stich zu bekommen oder eine andere Farbe abwerfen. Mit diesem Hintergrund *schätzt* der Spieler, wie viele Stiche er mit seinen Karten bekommt. Es sind Ansagen von 0 bis 7 (oder 9 bei Spieleranzahl kleiner sieben) möglich.

Hierbei kommt auch die strategische Komponente ins Spiel, denn die nachfolgenden Spieler können die Ansagen der Vorherigen sehen und so ihre eigene Ansage anpassen. 

Der Schriftführer notiert die Ansagen nach und nach auf seinem Zettel (später in der App) und nachdem der Dealer seine Ansage gemacht hat, startet der zweite Abschnitt:

#### Das Spielen
Der Spieler **links vom Dealer** beginnt mit dem Ausspielen einer Karte. Dabei ist es vollkommen egal, was für eine Karte er ausspielt (Trumpf-Farbe oder nicht). Alle nachfolgenden Spieler müssen diese Farbe erwidern, sofern sie sie haben. Wenn nicht, darf eine Trumpf-Farbe ausgespielt werden, um zu signalisieren, dass **dieser Spieler** den Stich haben möchte. Er kann aber auch eine andere Farbe abwerfen, wenn er die Farbe nicht bedienen kann. Das bewusste Nichtbedienen ist ein Regelverstoß, der bis zum Spielausschluss geahndet werden kann.

Der Spieler, der entweder die höchste Karte der geforderten Farbe **oder** die höchste Trumpf-Farbe gelegt hat bekommt den Stich und ist nun an der Reihe, eine Karte zu legen. Dieses wiederholt sich so lange, bis kein Spieler mehr eine Karte auf der Hand hat. Die Stiche werden sorgfältig auf einem für den Spieler geeigneten Platz so hingelegt, dass man die Zahl der Stiche auf einen Blick sehen kann. 

Sind alle Stiche ausgespielt, geht es zum dritten Abschnitt:

#### Das Auswerten
Der Schriftführer zählt reihum, beginnend vom Spieler **links vom Dealer** die Stiche und vergleicht diese mit den Ansagen. Jeder Stich ist pauschal schon mal ein Punkt wert. Hat der Spieler genauso viele Stiche bekommen, wie er angesagt hat, bekommt dieser einen Bonus von 10 Punkten. Hat der Spieler mehr oder weniger Stiche als angesagt, bekommt er so viele Punkte, wie er Stiche bekommen hat.

##### Sonderfall: 0 Punkte angesagt und eingehalten
Hat der Spieler 0 Punkte angesagt und auch 0 Punkte erreicht, bekommt er 20 Punkte. Bei Nichteinhalten bekommt er so viele Punkte, wie er Stiche gesammelt hat.

Der Schriftführer notiert die Punkte auf dem Zettel (später in der App) und zählt die Punkte zusammen. [Ein Beispiel eines solchen Punktezettels findet sich im Anhang/Ordner "preparation".] Sobald ein Spieler 100 Punkte + Datum erreicht hat, ist die Runde zu Ende. 100 plus Datum heißt, wenn heute z.B. der 6.11. wäre, dann ist die Gewinnmarke 106 Punkte, die es zu erreichen gilt. Haben mehrere Spieler die Gewinnmarke erreicht, dann ist derjenige Spieler, der diese Marke zuerst erreicht hat, der Gewinner.

### Glossar der Spielbegriffe

| Begriff | Erklärung |
|---------|-----------|
| **Stich** | Eine Spielrunde, bei der jeder Spieler eine Karte legt. Der Spieler mit der höchsten Karte der ausgespielten Farbe oder der höchsten Trumpf-Farbe gewinnt den Stich. |
| **Trumpf-Farbe** | Die zu Beginn des Spiels durch eine aufgedeckte Karte festgelegte Farbe, die alle anderen Farben schlägt. |
| **Bedienen** | Die Pflicht, eine Karte der ausgespielten Farbe zu legen, wenn man diese besitzt. |
| **Dealer** | Der Kartengeber, der die Karten mischt und austeilt. Diese Rolle wechselt nach jeder Runde im Uhrzeigersinn. |
| **Ansagen** | Die Vorhersage eines Spielers, wie viele Stiche er in einer Runde zu machen glaubt. Basis für die spätere Punkteberechnung. |
| **Abwerfen** | Das Spielen einer Karte einer anderen Farbe, wenn man die geforderte Farbe nicht bedienen kann. |
| **Schriftführer** | Die Person, die die Ansagen und Punkte notiert und die Auswertung vornimmt. Diese Person nutzt anstelle von Zettel und Stift die App zum Erfassen der Daten. |
| **100 plus Datum** | Die Gewinnregel, bei der die zu erreichende Punktzahl 100 plus die Tageszahl des aktuellen Datums ist (z.B. 106 Punkte am 6. eines Monats). |

## Technische Anforderungen

### Technologiestack

Die Anwendung wird mit folgenden Technologien entwickelt:

- **Frontend**: 
  - React.js als Hauptframework
  - Vanilla-CSS für das Styling
  - JavaScript (ES6+) für die Funktionalität

- **Backend**: 
  - Vanilla-PHP für die Serverlogik
  - JWT-Bibliothek für die Authentifizierung

- **Datenbank**: 
  - MariaDB für die persistente Datenspeicherung

- **Entwicklungsumgebung**: 
  - Node.js als Entwicklungsserver
  - Less für CSS-Präprozessor
  - XAMPP für lokale Entwicklung
  - Concurrent-Ausführung von React, PHP und Less

### Kernfunktionalitäten

#### 1. Spielerverwaltung
- Benutzerprofile erstellen und verwalten
- Authentifizierung und Autorisierung
- Spielerstatistiken und -wertungen speichern
- Persönliche Einstellungen (Avatar, Benachrichtigungen)

#### 2. Spielablauf-Management
- Spielerauswahl und Dealer-Bestimmung
- Eingabe und Verfolgung von angesagten Stichen
- Eingabe der tatsächlich erzielten Stiche
- Automatische Punkteberechnung
- Dealer-Rotation und Spielfortschritt

#### 3. Organisations-Features
- Erstellung von Einzelspielen
- Verwaltung mehrerer Spielgruppen
- Einladungssystem für Spiele

#### 4. Statistik und Ranglisten
- Globale Einzelspieler-Ranglisten
- Spielerwertungen basierend auf vergangenen Spielen
- Detaillierte Spielstatistiken
- Ligatabellen

### Benutzeroberfläche

Die Benutzeroberfläche wird für Tablets und Desktop optimiert, mit Unterstützung für große Handys im Querformat. Die Hauptansicht des Spiels wird wie folgt strukturiert:

**Datum: 06.11.2025 (Ziel: 106 Punkte)**

<div class="table-container" style="overflow-x: auto;">

| Spieler ||||||||||| Ges. |
|---------|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| | **Runde #01** ||| **Runde #02** ||| **Runde #03** ||| **...** | |
| | A | S | P | A | S | P | A | S | P | | |
| Spieler 1 | 2 | 3 | 3 | 4 | 1 | 1 | 0 | 2 | 2 | ... | 076 |
| **Spieler 2*** | 0 | 1 | 1 | 1 | **1** | **11** | 3 | 2 | 2 | ... | **112** |
| Spieler 3 | 2 | **2** | **12** | 3 | 4 | 4 | 2 | **2** | **12** | ... | 107 |
| Spieler 4 | 3 | **3** | **13** | 0 | **0** | **20** | 2 | 1 | 1 | ... | 083 |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| Spieler x | 0 | **0** | **20** | 1 | **1** | **11** | 1 | **1** | **11** | ... | 098 |

</div>

**Legende:** A = Ansage, S = Stiche, P = Punkte dieser Runde, Ges = Gesamtpunkte  
* = Dealer in dieser Runde

Besonderheiten des UI-Designs:
- Fixierte Spalten für Spielernamen und Gesamtpunkte (bleiben immer sichtbar)
- Horizontal scrollbarer Bereich zwischen den fixierten Spalten, der alle Rundendetails enthält und bei vielen Runden ein horizontales Scrollen ermöglicht, während die Spielernamen und Gesamtpunkte stets sichtbar bleiben
- Farbliche Hervorhebung für:
  - Dealer der aktuellen Runde
  - Übereinstimmende Ansagen und erreichte Stiche
  - Gewinner (Spieler, der die Zielmarke zuerst erreicht)
- Responsive Anpassung für verschiedene Bildschirmgrößen

### Datenverwaltung

- **Persistente Speicherung**: Alle Spielergebnisse werden dauerhaft gespeichert
- **Datenstruktur**: Effiziente Datenbankstruktur für:
  - Spieler (ID, Name, Profilinformationen, Avatar)
  - Spiele (ID, Datum, Teilnehmer, Gewinner)
  - Runden (Spiel-ID, Rundennummer, Dealer)
  - Ergebnisse (Runden-ID, Spieler-ID, Ansage, Stiche, Punkte)
- **Skalierbarkeit**: Optimierte Abfragen für schnelle Datenverarbeitung auch bei großen Datenmengen

### Sicherheit und Datenschutz

- **Authentifizierung**: JWT-basierte Benutzerauthentifizierung
- **Autorisierung**: Rollenbasierte Zugriffsrechte (Spieler, Schriftführer, Administrator)
- **Datenschutz**: Konformität mit gängigen Datenschutzrichtlinien

### Benutzerrollen und Zugriffsrechte

#### Spielleiter
- Spiele erstellen und verwalten
- Spieler einladen und hinzufügen
- Spielverlauf dokumentieren (Ansagen, Stiche, Punkte)
- Spielergebnisse finalisieren
- Spielgruppen organisieren und verwalten

#### Spieler
- An Spielen teilnehmen
- Eigenes Profil verwalten (Avatar, Einstellungen)
- Persönliche Statistiken einsehen
- Ranglisten und Ligatabellen betrachten
- Spielhistorie ansehen
- Bei Bedarf als Spielleiter fungieren (wenn nicht in aktiver Partie)

#### Administrator
- Systemeinstellungen verwalten
- Benutzerkonten verwalten
- Globale Statistiken einsehen
- Technische Probleme beheben

### Rollenmanagement und Zugriffslogik

- **Dynamische Rollenzuweisung**:
  - Ein Benutzer kann zwischen Spieler- und Spielleiter-Rolle wechseln
  - Ist ein Spieler in einer aktiven Partie, kann er nicht gleichzeitig als Spielleiter fungieren
  - Nach Anmeldung kann ein Spieler, der nicht in einer aktiven Partie ist, zwischen "Spiel leiten" und "Spielerprofil" wählen

- **Spielleiter-Exklusivität**:
  - Zu jedem Zeitpunkt kann nur ein Spielleiter pro Spiel/Liga aktiv sein
  - Der Spielleiter bleibt aktiv, bis er sich explizit abmeldet
  - Bei Verbindungsverlust bleibt die Spielleiter-Rolle erhalten (Offline-Funktionalität)

- **Offline-Funktionalität**:
  - Lokale Zwischenspeicherung (Cookies/LocalStorage) für Verbindungsunterbrechungen
  - Synchronisierung mit dem Server, sobald die Verbindung wiederhergestellt ist

### Erweiterbarkeit

Die Anwendung wird modular aufgebaut, um zukünftige Erweiterungen zu erleichtern:

- **Spieler-Dashboard**: Persönlicher Bereich für jeden Spieler mit:
  - Übersicht über laufende und vergangene Spiele
  - Persönliche Statistiken und Erfolge
  - Einladungen zu neuen Spielen
  - Benachrichtigungen über Spielaktivitäten

- **Mehrsprachigkeit**: Vorbereitung für mehrsprachige Unterstützung

- **API-Schnittstellen**: Für potenzielle mobile Apps oder Drittanbieter-Integrationen

- **Exportfunktionen**: Für Spielstatistiken und Ergebnisse (PDF, CSV)

- **Spielvarianten**: Möglichkeit zur Erweiterung um weitere Spielmodi oder Regelanpassungen

- **Liga-System**:
  - Organisation von Ligen und Turnieren
  - Passwortgeschützte Liga-Verwaltung
  - Saisonale Wettbewerbe
  - Automatische Ranglisten für Ligen

- **Soziale Funktionen**: Freundeslisten, Direktnachrichten, Spielersuche