# pseudonymizePatient - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **pseudonymizePatient**

## OperationDefinition: pseudonymizePatient 

| | |
| :--- | :--- |
| *Official URL*:https://ths-greifswald.de/fhir/OperationDefinition/gpas/pseudonymizePatient | *Version*:2025.2.0 |
| Active as of 2026-02-18 | *Computable Name*:PseudonymizePatient |

## Zweck

Durchführung eines Record Linkage auf Basis von (reduzierten) Patient-Ressourcen und Abfrage/Erzeugung von entsprechenden Pseudonymen.

Grundlage für das Record Linkage sind die in der Patienten-Ressource enthaltenen jedoch stark begrenzten Informationen. Dies können sowohl personenidentifizierende Informationen (u.a. Name, Vorname, Geburtsdatum, Kontakt- oder Adressinformationen) oder auch nur Identifier (u.a. KVID10, Bloomfilter) sein. Im Ergebnis wird System-intern eine eineindeutige Personenkennung (Master Person Index) erzeugt. Anschließend werden entsprechend der gewünschten Anzahl Pseudonyme (Parameter **count**) erzeugt und in einem Ergebnis-Bundle zurückgegeben. Die Zuordnung von eingehender Patienten-Ressource und Ergebnis-Pseudonym(en) erfolgt über die eingehende **Patient.id**.

## Voraussetzung

* API-Key: Der spezifizierte API-Key muss valide und zum Aufruf der Methode autorisiert sein. Der API-KEY wird im Request-Header übermittelt.
* Die Patient-Ressource muss den Profilvorgaben **PseudonymizePatient** entsprechen.
* Die angegebene Pseudonym-Domäne muss konfiguriert sein.
* Im Fall von **count > 1**: Die angegebene Pseudonym-Domäne muss in der Lage sein mehre Pseudonyme für einen Originalwert zu verwalten (Multi-Psn-Domäne).
* Es wird nur der Bundle.Type **batch** unterstützt.

## Aufruf und Rückgabe

Im Kontext dieser Operation wird das [PatientPseudonymized-Profil](StructureDefinition-PatientPseudonymized.md) verwendet.

Bei count = 0 wird nur lesend zugegriffen und werden keine Pseudonyme erzeugt. Bei count > 1 ist die Konfiguration von Multi-Psn-Domänen erforderlich. In diesem Fall kann die Rückgabe mehrere Parameter mit dem Bezeichner pseudonym enthalten.

Im Fehlerfall wird eine OperationOutcome-Ressource mit entsprechenden Informationen zurückgegeben. Bei Verwendung innerhalb eines Batch-Bundles (siehe Beispiele) wird in der Batch-Response neben diesem OperationOutcome auch eine Parameters-Ressource zurückgegeben, die auf die betroffene PatientId sowie das Target verweist.

## Beispiel

* [Request-Body](Bundle-PseudonymizePatient-Bundle-request-example-1.md)
* [Rückmeldung](Bundle-PseudonymizePatient-Bundle-response-example-1.md)



## Resource Content

```json
{
  "resourceType" : "OperationDefinition",
  "id" : "PseudonymizePatient",
  "url" : "https://ths-greifswald.de/fhir/OperationDefinition/gpas/pseudonymizePatient",
  "version" : "2025.2.0",
  "name" : "PseudonymizePatient",
  "title" : "pseudonymizePatient",
  "status" : "active",
  "kind" : "operation",
  "date" : "2026-02-18",
  "publisher" : "Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "contact" : [{
    "name" : "Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
    "telecom" : [{
      "system" : "url",
      "value" : "https://www.ths-greifswald.de/"
    }]
  }],
  "affectsState" : true,
  "code" : "pseudonymizePatient",
  "comment" : "Abfrage von 1-n eines Pseudonym-Werten für einen Originalwert und eine spezifische Domäne. Eine gleichzeitige Verarbeitung von mehreren Pseudonymisierungen kann durch Übergabe mehrerer entsprechender Requests in einem FHIR-Batch-Bundle erfolgen.",
  "system" : true,
  "type" : false,
  "instance" : false,
  "parameter" : [{
    "name" : "study",
    "use" : "in",
    "min" : 1,
    "max" : "1",
    "documentation" : "Angabe der Studie auf Basis derer für die angegebenen Originalwerte vorhandene Pseudonyme gesucht und ggf. erzeugt werden",
    "type" : "string"
  },
  {
    "name" : "patient",
    "use" : "in",
    "min" : 1,
    "max" : "1",
    "documentation" : "Patienten-Ressource des Patienten, für die 1-n Pseudonyme erzeugt werden sollen",
    "type" : "Patient"
  },
  {
    "name" : "context",
    "use" : "in",
    "min" : 1,
    "max" : "*",
    "documentation" : "Kontext der zu generierenden oder zu suchenden Pseudonyme.",
    "part" : [{
      "name" : "target",
      "use" : "in",
      "min" : 1,
      "max" : "1",
      "documentation" : "Angabe der Pseudonymisierungs-Domäne in welcher nach vorhandenen Pseudonymen gesucht wird oder neue Pseudonyme erzeugt werden sollen.",
      "type" : "string"
    },
    {
      "name" : "count",
      "use" : "in",
      "min" : 0,
      "max" : "1",
      "documentation" : "Angabe der Anzahl zu erzeugender Pseudonyme innerhalb der Domäne. Default = 1.",
      "type" : "integer"
    }]
  },
  {
    "name" : "externalPatientId",
    "use" : "out",
    "min" : 1,
    "max" : "1",
    "documentation" : "ID der Patient-Ressource zum Zweck der Rückreferenzierung. Es wird die vom Client übermittelte ID (Element Patient.id) verwendet, in Anlehnung an das Konzept 'Update as Create' as der FHIR-Spezifikation.",
    "type" : "string"
  },
  {
    "name" : "pseudonym",
    "use" : "out",
    "min" : 1,
    "max" : "*",
    "documentation" : "Gruppierung der domänenspezifischen Pseudonyme.",
    "part" : [{
      "name" : "target",
      "use" : "out",
      "min" : 1,
      "max" : "1",
      "documentation" : "Angabe der Domäne (entspricht dem beim Request übermittelten Wert) zum Zweck der Rückreferenzierung",
      "type" : "Identifier"
    },
    {
      "name" : "value",
      "use" : "out",
      "min" : 0,
      "max" : "*",
      "documentation" : "Das erzeugte Pseudonym (wird nur im Erfolgsfall übermittelt).",
      "type" : "Identifier"
    }]
  }]
}

```
