Der FHIR-Endpunkt (```base```) für die übergreifende Schnittstelle lautet

<strong>```http[s]://\<host\>:\<port\>/ttp-fhir/fhir/dispatcher```</strong>

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
