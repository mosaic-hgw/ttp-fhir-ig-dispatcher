# requestPsnWorkflow - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **requestPsnWorkflow**

## OperationDefinition: requestPsnWorkflow 

| | |
| :--- | :--- |
| *Official URL*:https://ths-greifswald.de/fhir/OperationDefinition/dispatcher/requestPsnWorkflow | *Version*:2025.2.0 |
| Active as of 2026-02-18 | *Computable Name*:RequestPsnWorkflow |

 
Abfragen bzw. anlegen von Pseudonymen auf Basis eines vorkonfigurierten Pseudonymisierungsablaufs (Workflow) für einen gegebenen Geltungsbereich (Studie und Standort). Die Rückgabe der generierten standort- und studienspezifischen-Pseudonyme erfolgt als Parameter. 

## Zweck

Abfragen bzw. Anlegen von Pseudonymen auf Basis eines vorkonfigurierten Pseudonymisierungsablaufs (Workflow) für einen gegebenen Geltungsbereich (Studie und Standort).

Dabei wird stets ein oder mehrere Originalwerte einer Quell-Domäne in ein oder mehrere Pseudonyme der Ziel-Domäne pseudonymisiert. Ist der Originalwert bereits bekannt, wird das bereits zuvor generierte Pseudonym der Ziel-Domäne geliefert.

Diese Methode überführt Pseudonyme einer Stufe in eine andere Stufe. Dabei werden entweder bekannte Pseudonyme zurückgeliefert (Um-Pseudonymisierung) oder neue Pseudonyme generiert (Dritt-Pseudonymisierung).

Die Rückgabe der generierten standort- und studienspezifischen Pseudonyme erfolgt als Parameter.

 ![](assets/images/fhirgw-requestpsnworkflow.png) 

## Voraussetzung

* API-Key: Der spezifizierte API-Key muss valide und zum Aufruf der Methode autorisiert sein. Der API-KEY wird im Request-Header übermittelt.
* Die spezifizierte Studie muss im Zielsystem bekannt und angelegt sein.
* Die spezifizierte Quell-Domäne (source) muss im Zielsystem bekannt und angelegt sein.
* Die standortspezifische Domäne (target) muss im Zielsystem bekannt und angelegt sein.
* Das angegebene Event muss bekannt sein und der API-Key dafür autorisiert sein.

## Aufruf und Rückgabe

Die bereitgestellte Funktionalität kann per POST-Request aufgerufen werden. Die erforderlichen Angaben werden per POST-BODY in Form von [FHIR Parameters](https://www.hl7.org/fhir/parameters.html) übermittelt.

`<HOST>:<PORT>/ttp-fhir/fhir/dispatcher/$requestPsnWorkflow`

Der Funktionsaufruf liefert eine Parameters-Ressource bestehend aus multiplen Multi-Part-Parametern zurück.

Im Erfolgsfall wird ein pseudonym-Parameter pro übergebenen Originalwert zurückgegeben, welcher folgende Parameter enthält:

1. original = der zu pseudonymisierende Wert (im Request übergeben)
1. target = die verwendete Ziel-Domäne (im Request übergeben)
1. pseudonym = Das in der Ziel-Domäne erzeugte Pseudonym.

Im Erfolgsfall wird der HTTP Statuscode 200 zurückgegeben.

Wenn einzelne übergebene Parameter fehlerhaft bzw. nicht valide sind, wird statt eines Pseudonyms ein Fehler-Parameter (error-Parameter) mit der Fehlerbeschreibung zurückgeliefert.

Ist der Request gänzlich ungültig, wird einer der folgenden HTTP Statuscodes in Verbindung mit einer OperationOutcome-Ressource zurückgegeben:

* 400: Fehlende oder fehlerhafte Parameter.
* 401: Fehlende Authentifizierung oder Autorisierung.
* 404: Parameter mit unbekanntem Inhalt.
* 422: Fehlende oder falsche Patienten-Attribute.

## Beispiel

* [Request-Body](Parameters-Parameters-RequestPsnWorkflow-request-example-1.md)
* [Rückmeldung](Parameters-Parameters-RequestPsnWorkflow-response-example-1.md)



## Resource Content

```json
{
  "resourceType" : "OperationDefinition",
  "id" : "RequestPsnWorkflow",
  "url" : "https://ths-greifswald.de/fhir/OperationDefinition/dispatcher/requestPsnWorkflow",
  "version" : "2025.2.0",
  "name" : "RequestPsnWorkflow",
  "title" : "requestPsnWorkflow",
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
  "description" : "Abfragen bzw. anlegen von Pseudonymen auf Basis eines vorkonfigurierten Pseudonymisierungsablaufs (Workflow) für einen gegebenen Geltungsbereich (Studie und Standort). Die Rückgabe der generierten standort- und studienspezifischen-Pseudonyme erfolgt als Parameter.",
  "code" : "requestPsnWorkflow",
  "comment" : "Abfragen bzw. anlegen von Pseudonymen auf Basis eines vorkonfigurierten Pseudonymisierungsablaufs (Workflow) für einen gegebenen Geltungsbereich (Studie und Standort). Die Rückgabe der generierten standort- und studienspezifischen-Pseudonyme erfolgt als Parameter.",
  "system" : true,
  "type" : false,
  "instance" : false,
  "parameter" : [{
    "name" : "original",
    "use" : "in",
    "min" : 1,
    "max" : "*",
    "documentation" : "Liste studien- und standortspezifischer Originalwerte für die entsprechende Pseudonyme ermittelt bzw. erstellt werden.",
    "type" : "string"
  },
  {
    "name" : "study",
    "use" : "in",
    "min" : 1,
    "max" : "1",
    "documentation" : "Angabe der Studie",
    "type" : "string"
  },
  {
    "name" : "source",
    "use" : "in",
    "min" : 1,
    "max" : "1",
    "documentation" : "Angabe der Quell-Domäne (Herkunft des Originalwertes)",
    "type" : "string"
  },
  {
    "name" : "target",
    "use" : "in",
    "min" : 1,
    "max" : "1",
    "documentation" : "Angabe der Ziel-Domäne",
    "type" : "string"
  },
  {
    "name" : "event",
    "use" : "in",
    "min" : 0,
    "max" : "1",
    "documentation" : "Optionaler Parameter. Auszulösendes, vorkonfiguriertes Pseudonymisierungsevents innerhalb des Workflow-Managers.",
    "type" : "string"
  },
  {
    "name" : "pseudonym",
    "use" : "out",
    "min" : 0,
    "max" : "*",
    "documentation" : "Ermitteltes bzw. generiertes studien- und standort-spezifisches Pseudonym",
    "part" : [{
      "name" : "original",
      "use" : "out",
      "min" : 1,
      "max" : "1",
      "documentation" : "der zu pseudonymisierende Wert (im Request übergeben)",
      "type" : "Identifier"
    },
    {
      "name" : "target",
      "use" : "out",
      "min" : 1,
      "max" : "1",
      "documentation" : "die verwendete Ziel-Domäne (im Request übergeben)",
      "type" : "Identifier"
    },
    {
      "name" : "pseudonym",
      "use" : "out",
      "min" : 1,
      "max" : "1",
      "documentation" : "das in der Ziel-Domäne erzeugte Pseudonym.",
      "type" : "Identifier"
    }]
  },
  {
    "name" : "error",
    "use" : "out",
    "min" : 0,
    "max" : "*",
    "documentation" : "Wenn einzelne übergebene Parameter fehlerhaft bzw. nicht valide sind, wird statt eines Pseudonyms ein Fehler-Parameter (error-Parameter) mit der Fehlerbeschreibung zurückgeliefert.",
    "part" : [{
      "name" : "original",
      "use" : "out",
      "min" : 0,
      "max" : "1",
      "documentation" : "der zu pseudonymisierende Wert (im Request übergeben)",
      "type" : "Identifier"
    },
    {
      "name" : "target",
      "use" : "out",
      "min" : 0,
      "max" : "1",
      "documentation" : "die verwendete Ziel-Domäne (im Request übergeben)",
      "type" : "Identifier"
    },
    {
      "name" : "error-code",
      "use" : "out",
      "min" : 1,
      "max" : "1",
      "documentation" : "Fehlercode",
      "type" : "Coding"
    }]
  }]
}

```
