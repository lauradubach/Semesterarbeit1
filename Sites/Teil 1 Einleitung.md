# Blob Storage & Azure Zertifizierung 

> Back [Page](https://github.com/lauradubach/Semesterarbeit1/blob/main/README.md)
>
> Next [Page](https://github.com/lauradubach/Semesterarbeit1/blob/main/Sites/Teil%202%20Vorbereitung.md)

- [Blob Storage \& Azure Zertifizierung](#blob-storage--azure-zertifizierung)
- [Versionenverzeichniss](#versionenverzeichniss)
- [Teil 1 Einleitung](#teil-1-einleitung)
- [Aufgabenstellung](#aufgabenstellung)
  - [Abgrenzung](#abgrenzung)
  - [Ausgangslage](#ausgangslage)
  - [Ziele](#ziele)
  - [Mittel und Methoden](#mittel-und-methoden)
    - [Software](#software)
    - [Programmiersprache](#programmiersprache)
  - [Werkzeuge](#werkzeuge)
  - [Methode IPERKA](#methode-iperka)
- [Projektorganisation](#projektorganisation)
  - [Beteiligte Personen](#beteiligte-personen)
    - [Kanditatin](#kanditatin)
    - [Dozenten](#dozenten)
- [Datensicherung](#datensicherung)
- [Zeitplan](#zeitplan)
- [Lernplan](#lernplan)
- [Besprechungsprotokoll](#besprechungsprotokoll)
    - [Besprechungsnotiz](#besprechungsnotiz)


# Versionenverzeichniss

| Version | Datum | Autor | Bemerkung | 
| ------- | ------ | ---- | --------- |
| 1.0 | 24.05.2024 | Laura Dubach | Inhaltsverzeichnis, Einleitung Dokumentation |
| 1.1 | 27.05.2024 | Laura Dubach | Titelseite, Weiterarbeit Einleitung Dokumentation, Verlinkung, Zeitplan und Lernplan erstellen |
| 1.2 | 28.05.2024 | Laura Dubach | Thema Informieren dokumentieren, Verlinkung, Zertifizierungstermin buchen |
| 1.3 | 30.05.2024 | Laura Dubach | Zeitplan -und Lernplan anpassen, start zusammenfassung AZ-900 Module |
| 1.4 | 31.05.2024 | Laura Dubach | Besprechungsprotokoll schreiben, Notizen im Notion machen |
| 1.5 | 03.06.2024 | Laura Dubach | Kapitel Planung dokumentiert, Kapitel Entscheiden gestartet |
| 1.6 | 05.06.2024 | Laura Dubach | Quellenverzeichniss nachführen, Entscheidungsmatrix starten |


# Teil 1 Einleitung
Mit der erfolgreichen Umsetzung dieses Projekts wird das Unternehmen in der Lage sein, große Datenmengen effizient, sicher und kostengünstig zu speichern und zu verwalten. Dies führt zu einer verbesserten Datenverfügbarkeit, niedrigeren Betriebskosten und einer erhöhten Gesamteffizienz im Datenmanagement.

# Aufgabenstellung
Das Projekt umfasst eine umfassende Analyse der aktuellen Speicheranforderungen von Unternehmen. Besonderheiten und Herausforderungen von Big Data, wie Volumen, Geschwindigkeit und Vielfalt der Daten, werden ebenfalls beleuchtet. Es erfolgt eine Bewertung von zwei verschiedenen Speichertechnologien im Kontext von Big Data, wobei Vor- und Nachteile detailliert erarbeitet werden. Auf Basis dieser Analyse wird ein Implementierungsplan für die beste Speicherlösung erstellt. Dieser Plan beinhaltet die praktische Implementierung und Verwaltung der Lösung sowie spezifische Verwaltungsherausforderungen und -lösungen. Die ausgewählte Speicherlösung ist Azure Blob Storage, das Flexibilität, Skalierbarkeit und Kosteneffizienz bietet. Ein weiterer Bestandteil des Projekts ist der Lernweg der HF Lernenden, um die Azure Fundamentals Zertifizierung zu erlangen. Dies stellt sicher, dass die Lernende die Azure-Umgebung effektiv nutzen und verwalten kann.

## Abgrenzung

1. Berechtigungskonzept gehört nicht zu diesem Projekt dazu
2. Das Backup vom BlobStorage wird im diesen Projekt nicht angewendet oder beschrieben
3. Die erfolgreiche Absolvierung der AZ-900 Zertifizierung ist nicht erforderlich, jedoch wird der Lernweg und die Vorbereitung beschrieben

## Ausgangslage
Viele Unternehmen stehen vor der Herausforderung, große Mengen an Daten effizient und kostengünstig zu speichern und zu verwalten. Die traditionellen Speichermethoden sind oft nicht skalierbar, teuer und schwierig zu sichern und zu verwalten. Unternehmen benötigen eine Lösung, die nicht nur skalierbar und kosteneffizient ist, sondern auch hohe Verfügbarkeit, Sicherheit und einfache Verwaltung bietet. 

## Ziele
1. Analyse der aktuellen Speicheranforderungen von Unternehmen
   - Erhebung und Darstellung der spezifischen Bedürfnisse von Unternehmen hinsichtlich Datenvolumen, Zugriffszeiten und Sicherheit. 
   - Besonderheiten und Herausforderungen von Big Data (z. B. Volumen, Geschwindigkeit, Vielfalt, Auswertung). 

2. Analyse und Bewertung von Speichertechnologien im Kontext von Big Data 
   - Eine Analyse von zwei Storages durchführen. 
   - Erarbeitung der Vor- und Nachteile der Storages 

3. Praktische Implementierung und Verwaltung: 
   - Erarbeitung eines Implementierungsplans für eine ausgewählte Speicherlösung. 
   - Darstellung der Verwaltungswerkzeuge und -prozesse für den laufenden Betrieb. 
   - Spezifische Verwaltungsherausforderungen und -lösungen für Big Data. 

4. Azure Fundamentales Zertifizierung 
   - Lernprozess beschreiben

## Mittel und Methoden
### Software
- Azure Portal
- Microsoft Azure Storage Explorer

### Programmiersprache
- CLI (bash)

## Werkzeuge
- Visio
- Excel
- github
- Visual Studio Code
- Chat GPT
- Microsoft Learn
- Ganttproject
- Notion

## Methode IPERKA
Dies ist eine Sechs-Schritte-Methode, welche man für die Umsetzung eines Projektes verwendet. Sie hilft dabei, ein Projekt von Grund auf gut zu planen und zu verstehen. Man soll jeden Schritt genau durchführen, um jegliche Probleme umgehen zu können. Zum Schluss der Methode wird auch verlangt, dass man das Projekt reflektiert, um aus allfälligen Fehlern auch lernen zu können. (Bexio 2020)

![IPERKA](/Semesterarbeit1/Pictures/iperka.jpg)

Für diese Methode habe ich mich entschieden, da wir diese in meiner Lehre für alle Projekte angewandt haben und ich gute Erfahrungen damit gemacht habe. Dadurch kenne ich diese Methode schon gut und kann sie dementsprechend anwenden.

# Projektorganisation
## Beteiligte Personen

### Kanditatin

```
Laura Joana Dubach
P: 079 355 78 24
Github: lauradubach
E-Mail: laura.dubach@itnetx.ch
```
### Dozenten

```
Philipp Rohr
Github: phrohr
E-Mail: philipp.rohr@tbz.ch
```
```
Samuel Müller
Github: 404samnotfound
E-Mail: samuel.mueller1@tbz.ch
```
```
Thanam Pangri
Github: tpangri
E-Mail: thanam.pangri@tbz.ch
```

# Datensicherung
Damit keine Daten verloren gehen können, werde ich alle Dokumente, auf meinem OneDrive abspeichern. Zusätzlich werde ich die Daten auf einen USB-Stick abspeichern, damit ich im Worstcase Szenario immer noch ein Backup besitze. 

# Zeitplan

![Zeitplan](../Pictures/Zeitplan.png)

# Lernplan

![Lernplan](../Pictures/Lernplan.png)

# Besprechungsprotokoll

| Besprechung | Datum | Uhrzeit | Teilnehmer | 
| ---- | ---- | ---- | ---- |
| 1 | 31.05.2024 | 18:15 - 18:30 | Philipp Rohr, Laura Dubach |

### Besprechungsnotiz

Vor dem Gespräch habe ich mir einige Gedanken gemacht, was für Fragen ich stellen möchte. Diese habe ich mir dann im Notion notiert.

1. Darf ich ChatPT für meine texte verwenden
2. Kunde erfinden oder allgemein schreiben
3. Wie soll ich AZ-900 integrieren 

Danach habe ich mich mit Philipp über Teams getroffen. Er meinte ChatGPT soll ich unbedingt verwenden, da es auch Zukunft ist. Wichtig ist einfach, dass ich die Quellen angebe. Zum Thema wie ich den Kunde einbauen soll, meinte er, am besten einen Kunden zu erfinden. So kann ich alles besser beschreiben und es gibt keine Verwirrungen. Zur letzten Frage wie ich die Zertifizierung einfliessen lassen soll, sagte er, ich soll meinen Lernweg aufzeigen und dann einen fliessenden Übergang zu meinem Thema machen, welches in der Lernunterlagen des AZ-900 aufzufinden ist. 

Das Gespräch war sehr gut und Philipp konnte all meine Fragen beantworten. So kann ich meine Smesterabreit nun gut weiterführen.

| Besprechung | Datum | Uhrzeit | Teilnehmer | 
| ---- | ---- | ---- | ---- |
| 2 | 24.06.2024 | 18:00 | Philipp Rohr, Laura Dubach |

Besprechungsnotiz

| Besprechung | Datum | Uhrzeit | Teilnehmer | 
| ---- | ---- | ---- | ---- |
| 3 | 1.07.2024 | 18:00 | Philipp Rohr, Laura Dubach |

Besprechungsnotiz
