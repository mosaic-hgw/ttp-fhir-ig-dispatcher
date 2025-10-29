#### Aufruf und Rückgabe
Die bereitgestellte Funktionalität kann per POST-Request aufgerufen werden. Die erforderlichen Angaben werden per POST-BODY in Form von [FHIR Parameters](https://www.hl7.org/fhir/parameters.html) übermittelt.

`<HOST>:<PORT>/ttp-fhir/fhir/dispatcher/$requestPsnFromBfWorkflow`

Der Funktionsaufruf liefert eine Parameters-Ressource bestehend aus multiplen Multi-Part-Parametern zurück.

Im Erfolgsfall wird der HTTP Statuscode 200 zurückgegeben.

Wenn einzelne übergebene Parameter fehlerhaft bzw. nicht valide sind, wird statt eines Pseudonyms ein Fehler-Parameter (error-Parameter) mit der Fehlerbeschreibung zurückgeliefert.

Ist der Request gänzlich ungültig, wird einer der folgenden HTTP Statuscodes in Verbindung mit einer OperationOutcome-Ressource zurückgegeben:
* 400: Fehlende oder fehlerhafte Parameter.
* 401: Fehlende Authentifizierung oder Autorisierung.
* 404: Parameter mit unbekanntem Inhalt.
* 422: Fehlende oder falsche Patienten-Attribute.

#### Hinweis zu zukünftigen Änderungen
Das Pseudonym wird künftig nur dann geliefert, wenn kein Clearing-Prozess angestoßen wird. Ist dieser erforderlich, muss dieser zunächst vollständig abgeschlossen sein und das Pseudonym kann über [die Operation $requestTasks](OperationDefinition-RequestTasks.html) abgerufen werden.

#### Beispiel

* [Request-Body](Parameters-Parameters-RequestPsnFromBfWorkflow-request-example-1.html)
* [Rückmeldung](Parameters-Parameters-RequestPsnFromBfWorkflow-response-example-1.html)
