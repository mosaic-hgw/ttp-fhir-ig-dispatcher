# pseudonymizePatient - v2025.1.0



## Resource Content

```json
{
  "resourceType" : "OperationDefinition",
  "id" : "PseudonymizePatient",
  "url" : "https://ths-greifswald.de/fhir/OperationDefinition/gpas/pseudonymizePatient",
  "version" : "2025.1.0",
  "name" : "PseudonymizePatient",
  "title" : "pseudonymizePatient",
  "status" : "active",
  "kind" : "operation",
  "date" : "2025-06-12",
  "publisher" : "Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "contact" : [
    {
      "name" : "Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
      "telecom" : [
        {
          "system" : "url",
          "value" : "https://www.ths-greifswald.de/"
        }
      ]
    }
  ],
  "affectsState" : true,
  "code" : "pseudonymizePatient",
  "comment" : "Abfrage von 1-n eines Pseudonym-Werten für einen Originalwert und eine spezifische Domäne. Eine gleichzeitige Verarbeitung von mehreren Pseudonymisierungen kann durch Übergabe mehrerer entsprechender Requests in einem FHIR-Batch-Bundle erfolgen.",
  "system" : true,
  "type" : false,
  "instance" : false,
  "parameter" : [
    {
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
      "part" : [
        {
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
        }
      ]
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
      "part" : [
        {
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
        }
      ]
    }
  ]
}

```
