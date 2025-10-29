#### Aufruf und Rückgabe
Die bereitgestellte Funktionalität kann per POST-Request aufgerufen werden. Die erforderlichen Angaben werden per POST-BODY in Form von [FHIR Parameters](https://www.hl7.org/fhir/parameters.html) übermittelt.

`<HOST>:<PORT>/ttp-fhir/fhir/dispatcher/$updateBf`

Der Funktionsaufruf liefert eine OperationOutcome-Ressource mit codierter Statusinformationen zurück.

Im Erfolgsfall wird der HTTP Statuscode 200 zurückgegeben.

Im vollständigen Fehlerfall wird einer der folgenden HTTP Statuscodes in Verbindung mit einer OperationOutcome-Ressource zurückgegeben:
* 400: Fehlende oder fehlerhafte Parameter.
* 401: Fehlende Authentifizierung oder Autorisierung.
* 404: Parameter mit unbekanntem Inhalt.
* 422: Fehlende oder falsche Patienten-Attribute.

#### Beispiel

* [Request-Body](Parameters-Parameters-UpdateBf-request-example-1.html)
* [Rückmeldung](Parameters-Parameters-UpdateBf-response-example-1.html)
