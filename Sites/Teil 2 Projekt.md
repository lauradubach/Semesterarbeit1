# Teil 2 Projekt

> Back [Page](/Semesterarbeit1/Sites/Teil%201%20Einleitung.md)
>
> Next [Page](/Semesterarbeit1/Sites/Teil%203%20Realisieren.md)

- [Teil 2 Projekt](#teil-2-projekt)
- [Informieren](#informieren)
  - [Bedürfnisse der Unternehmen](#bedürfnisse-der-unternehmen)
    - [Datenvolumen](#datenvolumen)
    - [Zugriffszeiten](#zugriffszeiten)
    - [Sicherheit](#sicherheit)
    - [Zusammenfassung](#zusammenfassung)
  - [Beschreibung Big Data](#beschreibung-big-data)
    - [Fazit](#fazit)
  - [Vorbereitung Zertifizierung](#vorbereitung-zertifizierung)
- [Planen](#planen)
  - [Ist Situation](#ist-situation)
  - [Soll Situation](#soll-situation)
  - [Umgebung](#umgebung)
- [Entscheiden](#entscheiden)
  - [Produkt Vergleich](#produkt-vergleich)
    - [Google Cloud Storage](#google-cloud-storage)
    - [Azure Blob Storage](#azure-blob-storage)
    - [Vor -und Nachteile](#vor--und-nachteile)
  - [Kostenanalyse](#kostenanalyse)
  - [Entscheidungsmatrix](#entscheidungsmatrix)


# Informieren
In diesem Kapitel werde ich Informationen zu meiner Arbeit beschaffen und diese erläutern.

## Bedürfnisse der Unternehmen
Unternehmen haben spezifische Anforderungen an Datenvolumen, Zugriffszeiten und Sicherheit, die je nach Branche, Größe und Geschäftsmodell variieren. Hier ist eine detaillierte Beschreibung dieser Bedürfnisse und wie sie typischerweise erhoben und dargestellt werden:

### Datenvolumen
   - Geschäftsanforderungen: Unternehmen analysieren ihre operativen Prozesse, Kundendaten und Markttrends, um das benötigte      Datenvolumen zu ermitteln. 
   - Zukünftiges Wachstum: Prognosen und Szenarioanalysen helfen bei der Abschätzung zukünftiger Datenmengen basierend auf Unternehmenswachstum und digitalen Transformationen.
   - Branchenvergleiche: Benchmarking gegen andere Unternehmen der Branche kann Aufschluss über übliche Datenvolumina geben.
   - Kapazitätsplanung: Erstellung von Berichten, die den aktuellen und prognostizierten Speicherbedarf darstellen, oft visualisiert durch Diagramme und Grafiken.
   - Datenstrategie-Dokumente: Detaillierte Strategien, die die kurz- und langfristigen Speicheranforderungen sowie Skalierungspläne enthalten.

### Zugriffszeiten
   - Anforderungsanalyse: Durchführung von Anforderungsanalysen bei verschiedenen Abteilungen (z. B. Marketing, Vertrieb, Produktion), um die benötigten Zugriffszeiten zu bestimmen.
   - Performance-Tests: Simulation von Datenzugriffen und Auswertungen der Reaktionszeiten, um die Anforderungen an Echtzeit- oder Batch-Verarbeitung zu verstehen.
   - Nutzerfeedback: Einholen von Feedback von Endbenutzern und IT-Teams, um Engpässe und Optimierungsbedarfe zu identifizieren.
   - Service-Level-Agreements (SLAs): Dokumentation von SLAs, die genaue Zugriffszeiten und Performance-Kriterien festlegen.
   - Dashboards: Nutzung von Dashboards zur Echtzeit-Überwachung der Systemperformance und Zugriffszeiten, um Transparenz und schnelle Reaktionsmöglichkeiten zu gewährleisten.

### Sicherheit
   - Risikobewertung: Durchführung von Risikoanalysen, um potenzielle Sicherheitsbedrohungen und Schwachstellen zu identifizieren.
   - Regulatorische Anforderungen: Berücksichtigung von branchenspezifischen Vorschriften und gesetzlichen Anforderungen (z. B. GDPR, HIPAA).
   - Sicherheitsaudits: Regelmäßige Sicherheitsaudits und Penetrationstests zur Überprüfung der aktuellen Sicherheitsmaßnahmen und Identifikation von Verbesserungsmöglichkeiten.
   - Sicherheitsrichtlinien: Erstellung und Aktualisierung umfassender Sicherheitsrichtlinien, die alle Aspekte des Datenmanagements abdecken.
   - Berichte und Dashboards: Regelmäßige Berichterstattung über Sicherheitsvorfälle und -maßnahmen, oft unterstützt durch Dashboards, die Echtzeit-Überwachung ermöglichen.

### Zusammenfassung
Unternehmen müssen ihre spezifischen Bedürfnisse hinsichtlich Datenvolumen, Zugriffszeiten und Sicherheit klar verstehen und darstellen, um ihre IT-Infrastruktur effizient zu planen und zu verwalten. Diese Bedürfnisse werden durch detaillierte Analysen, Simulationen und Nutzerfeedback erhoben und durch strukturierte Dokumentationen, Dashboards und Berichte visualisiert und kommuniziert. Durch die sorgfältige Erhebung und Darstellung dieser Anforderungen können Unternehmen sicherstellen, dass ihre Datenstrategien effektiv, skalierbar und sicher sind.
(Chat GPT)

## Beschreibung Big Data
Big Data ist ein Begriff, der die große Menge, Geschwindigkeit und Vielfalt an Daten beschreibt, die Unternehmen und Organisationen heutzutage verarbeiten und analysieren müssen. Die Besonderheiten und Herausforderungen von Big Data lassen sich in vier Hauptdimensionen zusammenfassen: Volumen, Geschwindigkeit, Vielfalt und Auswertung.

| **Aspekt** | **Besonderheiten** | **Herausforderungen** |
|----------------|-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
| **Volumen** | - Enorme Menge an Daten aus sozialen Medien, Transaktionsdaten, Sensoren, etc. | - Speicherung: Erfordert spezialisierte, kosteneffiziente und skalierbare Speicherlösungen |
| | - Moderne Technologien wie IoT und Internetnutzung treiben das Datenwachstum an | - Verwaltung: Benötigt robuste Datenmanagement-Systeme für Zugänglichkeit, Sicherheit und Organisation |
| **Geschwindigkeit** | - Daten müssen oft in Echtzeit oder nahezu in Echtzeit verarbeitet werden | - Verarbeitung in Echtzeit: Erfordert leistungsstarke und effiziente Datenverarbeitungstechnologien |
| | - Beispiele: Finanztransaktionen, Online-Werbung, Überwachungsdaten | - Latenzzeit: Minimierung der Latenzzeit ist entscheidend für rechtzeitige Entscheidungsfindung |
| **Vielfalt** | - Verschiedene Datenformen: strukturierte, unstrukturierte und semi-strukturierte Daten | - Integration: Komplexität der Integration unterschiedlicher Datenquellen und -formate |
| | - Quellen: Soziale Medien, Mobilgeräte, Sensoren, Unternehmenssysteme | - Analyse: Erfordert fortschrittliche Techniken wie maschinelles Lernen und natürliche Sprachverarbeitung |
| **Auswertung** | - Analyse und Interpretation von aten zur Gewinnung wertvoller Erkenntnisse | - Datenqualität: Sicherstellung der Genauigkeit und Zuverlässigkeit der Daten |
| | - Techniken: Data Mining, maschinelles Lernen, statistische Analysen | - Datenschutz: Schutz der Privatsphäre und Einhaltung von Datenschutzgesetzen |
| |                                                         | - Fachwissen: Bedarf an spezialisierten Fachkräften für Big Data-Technologien und -Methoden |

Diese Tabelle bietet eine klare und strukturierte Darstellung der verschiedenen Aspekte von Big Data, einschließlich ihrer besonderen Merkmale und der damit verbundenen Herausforderungen.

### Fazit
Big Data bietet enorme Möglichkeiten, bringt aber auch erhebliche Herausforderungen mit sich. Unternehmen und Organisationen müssen in geeignete Technologien, Prozesse und Fachkräfte investieren, um das Potenzial von Big Data voll auszuschöpfen und gleichzeitig die damit verbundenen Herausforderungen zu bewältigen.
 (Chat GPT)

## Vorbereitung Zertifizierung
Um mich gut auf die Zertifizierung vorzubereiten, werde ich als einen Lernplan erstellen.

Folgende punkte werde ich verfolgen:
  1. Alle Module im Microsoft Learn abschliessen
  2. Jedes Modul Zusammenfassen und in einem Repo dokumentieren
  3. Die Probeprüfung im Microsoft Learn absolvieren und üben
  4. Wenn nötig Braindups kaufen und mit diesen weiterlernen
  5. Bei Dozenten um ratschläge un Tipps fragen

# Planen
## Ist Situation
## Soll Situation
## Umgebung
# Entscheiden
## Produkt Vergleich
### Google Cloud Storage
### Azure Blob Storage
### Vor -und Nachteile
## Kostenanalyse
## Entscheidungsmatrix
