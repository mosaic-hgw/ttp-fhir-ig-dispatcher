# Artifacts Summary - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* **Artifacts Summary**

## Artifacts Summary

This page provides a list of the FHIR artifacts defined as part of this implementation guide.

### Behavior: Operation Definitions 

These are custom operations that can be supported by and/or invoked by systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [providePatientData](OperationDefinition-ProvidePatientData.md) | Identifizierende Daten (IDAT) werden für einen Clearing-Prozess an die föderierte Treuhandstelle (fTTP) übertragen. Die darin enthaltenen Attribute (z.B. Vorname, Nachname, usw.) dienen für ein konventionelles Record Linkage und werden danach in der fTTP unwiederbringlich gelöscht. |
| [pseudonymizePatient](OperationDefinition-PseudonymizePatient.md) |  |
| [requestPsnFromBfWorkflow](OperationDefinition-RequestPsnFromBfWorkflow.md) | Personenregistrierung und Privacy-Preserving Record Linkage (PPRL) auf Basis von Bloomfiltern (BF) innerhalb eines Geltungsbereiches (Studie, Standort). Die Erzeugung eines standortspezifischen Pseudonyms erfolgt innerhalb der angegebenen Ziel-Domäne. Diese wird automatisch erzeugt, sofern noch nicht vorhanden. Die Rückgabe eines standortspezifischen Pseudonyms (z.B. DIZPseudonym) erfolgt als Parameter. |
| [requestPsnWorkflow](OperationDefinition-RequestPsnWorkflow.md) | Abfragen bzw. anlegen von Pseudonymen auf Basis eines vorkonfigurierten Pseudonymisierungsablaufs (Workflow) für einen gegebenen Geltungsbereich (Studie und Standort). Die Rückgabe der generierten standort- und studienspezifischen-Pseudonyme erfolgt als Parameter. |
| [requestTasks](OperationDefinition-RequestTasks.md) | Abruf offener Standort-Aufgaben (Tasks) von der föderierten Treuhandstelle (fTTP). |
| [updateBf](OperationDefinition-UpdateBf.md) | Aktualisierung eines bestehenden Bloomfilters (z.B. bei geänderter Konfiguration oder vorheriger fehlerhafter Übermittlung) bezogen auf ein bereits bekanntes Pseudonym. |

### Structures: Resource Profiles 

These define constraints on FHIR resources for systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [IDAT](StructureDefinition-Idat.md) | Patienten-Profil zur Übermittlung von angeforderten IDAT an die fTTP für den Clearing-Prozess. |

### Terminology: Code Systems 

These define new code systems used by systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [BloomfilterType](CodeSystem-BloomfilterTypeCS.md) | Types of Bloomfilters. |

### Example: Example Instances 

These are example instances that show what data produced and consumed by systems conforming with this implementation guide might look like.

| |
| :--- |
| [Idat-example-1](Patient-Idat-example-1.md) |
| [OperationOutcome-UpdateBf-response-example-1](OperationOutcome-OperationOutcome-UpdateBf-response-example-1.md) |
| [Parameters-ProvidePatientData-request-example-1](Parameters-Parameters-ProvidePatientData-request-example-1.md) |
| [Parameters-RequestPsnFromBfWorkflow-request-example-1](Parameters-Parameters-RequestPsnFromBfWorkflow-request-example-1.md) |
| [Parameters-RequestPsnFromBfWorkflow-response-example-1](Parameters-Parameters-RequestPsnFromBfWorkflow-response-example-1.md) |
| [Parameters-RequestPsnWorkflow-request-example-1](Parameters-Parameters-RequestPsnWorkflow-request-example-1.md) |
| [Parameters-RequestPsnWorkflow-response-example-1](Parameters-Parameters-RequestPsnWorkflow-response-example-1.md) |
| [Parameters-RequestTasks-request-example-1](Parameters-Parameters-RequestTasks-request-example-1.md) |
| [Parameters-RequestTasks-response-example-1](Parameters-Parameters-RequestTasks-response-example-1.md) |
| [Parameters-UpdateBf-request-example-1](Parameters-Parameters-UpdateBf-request-example-1.md) |
| [PseudonymizePatient-Bundle-request-example-1](Bundle-PseudonymizePatient-Bundle-request-example-1.md) |
| [PseudonymizePatient-Bundle-response-example-1](Bundle-PseudonymizePatient-Bundle-response-example-1.md) |

