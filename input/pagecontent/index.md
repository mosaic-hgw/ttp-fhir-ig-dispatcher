# FHIR-Support für Übergreifende Schnittstellen

Stand 18.02.2026

Die Softwarelösungen E-PIX, gPAS, gICS und Dispatcher werden in zahlreichen Forschungseinrichtungen und Projekten für die Realisierung von Treuhandstellen-Services (THS) eingesetzt. Um die Verwendung dieser Lösungen in FHIR-basierten Infrastrukturen zu unterstützen, werden ausgewählte THS-Funktionalitäten durch FHIR-basierte Operations, Profile, Erweiterungen und Terminologien realisiert.

Diese werden in entsprechenden [Implementierungsleitfäden](https://www.ths-greifswald.de/fhir) themenspezifisch beschrieben und zahlreiche Details erläutert.

Der vorliegende **Implementation Guide Übergreifende Schnittstellen** setzt den Fokus auf Operations, Profile und Extensions, die für die [föderierte Treuhandstelle (fTTP)](https://www.ths-greifswald.de/dispatcher/fhir) relevant sind.
           
### Endpunkt

Der FHIR-Endpunkt (```base```) für die übergreifende Schnittstelle lautet

<strong>```http[s]://\<host\>:\<port\>/ttp-fhir/fhir/dispatcher```</strong>

Die Umsetzung komplexer Standort- und System-übergreifender Workflows erfordert wohldefinierte Schnittstellen. 
Im Kontext des **föderierten Record Linkage mittels fTTP** werden unterschiedliche HL7-FHIR Operations genutzt.

### Übersicht der fTTP-Operations

Nachfolgende Tabelle listet die zum aktuellen Zeitpunkt gültigen **fTTP**-Funktionalitäten ([federated Trusted Third Party](https://www.ths-greifswald.de/forscher/num/fttp-fact-sheet)).

| Operation|erforderlich für fTTP-Modul|
-- | ---
|[requestPsnWorkflow](OperationDefinition-requestPsnWorkflow.md)|Wahrscheinlichkeit|
|[requestPsnFromBfWorkflow](OperationDefinition-requestPsnFromBfWorkflow.md)|Wahrscheinlichkeit|
|[updateBf](OperationDefinition-updateBf.md)|Wahrscheinlichkeit|
|[requestTasks](OperationDefinition-requestTasks.md)|Wahrscheinlichkeit/Clearing|
|[providePatientData](OperationDefinition-providePatientData.md)|Clearing|


### Übersicht der generalisierten fTTP-Operations

| Operation                                                                                               | Zweck                                                  |
---------------------------------------------------------------------------------------------------------|--------------------------------------------------------
| [pseudonymizePatient](OperationDefinition-pseudonymizePatient.md) | Erzeugung von Pseudonym(en) für eine Patient-Ressource |

### Package

Das automatisch erzeugte Package (TGZ) steht als Download zur Verfügung unter: [Link](package.tgz).


### Implementierung

Peter Penndorf, Martin Bialke, Christoper Hampf, Frank Michael Moser

### Autoren

Martin Bialke, Stefan Lang

### Kontakt

kontakt-ths (at) med.uni-greifswald.de