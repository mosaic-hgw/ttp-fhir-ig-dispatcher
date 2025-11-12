# FHIR-Support für Übergreifende Schnittstellen

Stand 12.11.2025
           
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


### Implementierung

Peter Penndorf, Martin Bialke, Christoper Hampf, Frank Michael Moser

### Autoren

Martin Bialke, Stefan Lang

### Kontakt

kontakt-ths (at) uni-greifswald.de
