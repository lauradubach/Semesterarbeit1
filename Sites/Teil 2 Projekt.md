# Teil 2 Projekt

> Back [Page](/Semesterarbeit1/Sites/Teil%201%20Einleitung.md)
>
> Next [Page](/Semesterarbeit1/Sites/Teil%203%20Realisieren.md)

- [Teil 2 Projekt](#teil-2-projekt)
- [Informieren](#informieren)
  - [Bedürfnisse Unternehmen](#bedürfnisse-unternehmen)
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

## Bedürfnisse Unternehmen
Unternehmen haben spezifische Anforderungen an Datenvolumen, Zugriffszeiten und Sicherheit, die je nach Branche, Größe und Geschäftsmodell variieren. Hier ist eine detaillierte Beschreibung dieser Bedürfnisse und wie sie typischerweise erhoben und dargestellt werden:

1. Datenvolumen
   - Geschäftsanforderungen: Unternehmen analysieren ihre operativen Prozesse, Kundendaten und Markttrends, um das benötigte      Datenvolumen zu ermitteln. 
   - Zukünftiges Wachstum: Prognosen und Szenarioanalysen helfen bei der Abschätzung zukünftiger Datenmengen basierend auf Unternehmenswachstum und digitalen Transformationen.
   - Branchenvergleiche: Benchmarking gegen andere Unternehmen der Branche kann Aufschluss über übliche Datenvolumina geben.
   - Kapazitätsplanung: Erstellung von Berichten, die den aktuellen und prognostizierten Speicherbedarf darstellen, oft visualisiert durch Diagramme und Grafiken.
   - Datenstrategie-Dokumente: Detaillierte Strategien, die die kurz- und langfristigen Speicheranforderungen sowie Skalierungspläne enthalten.

2. Zugriffszeiten
   - Anforderungsanalyse: Durchführung von Anforderungsanalysen bei verschiedenen Abteilungen (z. B. Marketing, Vertrieb, Produktion), um die benötigten Zugriffszeiten zu bestimmen.
   - Performance-Tests: Simulation von Datenzugriffen und Auswertungen der Reaktionszeiten, um die Anforderungen an Echtzeit- oder Batch-Verarbeitung zu verstehen.
   - Nutzerfeedback: Einholen von Feedback von Endbenutzern und IT-Teams, um Engpässe und Optimierungsbedarfe zu identifizieren.
   - Service-Level-Agreements (SLAs): Dokumentation von SLAs, die genaue Zugriffszeiten und Performance-Kriterien festlegen.
   - Dashboards: Nutzung von Dashboards zur Echtzeit-Überwachung der Systemperformance und Zugriffszeiten, um Transparenz und schnelle Reaktionsmöglichkeiten zu gewährleisten.

3. Sicherheit
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

1. Volumen
**Besonderheiten:**
- Das Volumen von Daten bezieht sich auf die enorme Menge an Daten, die täglich generiert wird. Dies umfasst Daten aus sozialen Medien, Transaktionsdaten, Sensoren und mehr.
- Moderne Technologien wie IoT (Internet der Dinge) und die allgegenwärtige Nutzung des Internets tragen zur exponentiellen Zunahme der Datenmengen bei.

**Herausforderungen:**
- Speicherung: Die Speicherung riesiger Datenmengen erfordert spezialisierte Speicherlösungen, die sowohl kosteneffizient als auch skalierbar sind.
- Verwaltung: Die Verwaltung dieser Daten erfordert robuste Datenmanagement-Systeme, um sicherzustellen, dass die Daten zugänglich, sicher und organisiert sind.

2. Geschwindigkeit
**Besonderheiten:**
- Geschwindigkeit bezieht sich auf die Geschwindigkeit, mit der Daten generiert und verarbeitet werden müssen. In vielen Fällen müssen Daten in Echtzeit oder nahezu in Echtzeit verarbeitet werden.
- Beispiele sind Finanztransaktionen, Online-Werbung und Überwachungsdaten.

**Herausforderungen:**
- Verarbeitung in Echtzeit: Die Notwendigkeit, große Datenmengen in Echtzeit zu analysieren und darauf zu reagieren, erfordert leistungsstarke und effiziente Datenverarbeitungstechnologien.
- Latenzzeit: Minimierung der Latenzzeit ist entscheidend, um sicherzustellen, dass die Informationen rechtzeitig für Entscheidungsfindungen zur Verfügung stehen.

3. Vielfalt
**Besonderheiten:**
- Vielfalt bezieht sich auf die verschiedenen Formen und Quellen von Daten, einschließlich strukturierter Daten (z. B. Datenbanken), unstrukturierter Daten (z. B. Texte, Videos) und semi-strukturierter Daten (z. B. XML-Dateien).
- Daten stammen aus einer Vielzahl von Quellen wie sozialen Medien, Mobilgeräten, Sensoren, Unternehmenssystemen und mehr.

**Herausforderungen:**
- Integration: Die Integration unterschiedlicher Datenquellen und -formate in eine kohärente Datenstruktur ist komplex.
- Analyse: Die Analyse von unstrukturierten Daten erfordert fortschrittliche Techniken wie maschinelles Lernen und natürliche Sprachverarbeitung.

4. Auswertung
**Besonderheiten:**
- Die Auswertung von Big Data umfasst die Analyse und Interpretation der gesammelten Daten, um wertvolle Erkenntnisse zu gewinnen.
- Techniken wie Data Mining, maschinelles Lernen und statistische Analysen werden verwendet, um Muster zu erkennen und Vorhersagen zu treffen.

**Herausforderungen:**
- Datenqualität: Sicherstellung der Genauigkeit und Zuverlässigkeit der Daten ist entscheidend, da fehlerhafte Daten zu falschen Schlussfolgerungen führen können.
- Datenschutz: Der Schutz der Privatsphäre und die Einhaltung von Datenschutzgesetzen sind bei der Verarbeitung großer Datenmengen von großer Bedeutung.
- Fachwissen: Es besteht ein Bedarf an spezialisierten Fachkräften, die über das nötige Wissen und die Fähigkeiten verfügen, um Big Data-Technologien und -Methoden effektiv anzuwenden.

### Fazit
Big Data bietet enorme Möglichkeiten, bringt aber auch erhebliche Herausforderungen mit sich. Unternehmen und Organisationen müssen in geeignete Technologien, Prozesse und Fachkräfte investieren, um das Potenzial von Big Data voll auszuschöpfen und gleichzeitig die damit verbundenen Herausforderungen zu bewältigen.
 (Chat GPT)

## Vorbereitung Zertifizierung

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
