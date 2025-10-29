#### Aufruf und Rückgabe
Die bereitgestellte Funktionalität kann per POST-Request aufgerufen werden. Die erforderlichen Angaben werden per POST-BODY in Form von [FHIR Parameters](https://www.hl7.org/fhir/parameters.html) übermittelt.

`<HOST>:<PORT>/ttp-fhir/fhir/dispatcher/$requestPsnWorkflow`

Der Funktionsaufruf liefert eine Parameters-Ressource bestehend aus multiplen Multi-Part-Parametern zurück.

Im Erfolgsfall wird ein pseudonym-Parameter pro übergebenen Originalwert zurückgegeben, welcher folgende Parameter enthält:
1. original = der zu pseudonymisierende Wert (im Request übergeben)
2. target = die verwendete Ziel-Domäne (im Request übergeben)
3. pseudonym = Das in der Ziel-Domäne erzeugte Pseudonym.

Im Erfolgsfall wird der HTTP Statuscode 200 zurückgegeben.

Wenn einzelne übergebene Parameter fehlerhaft bzw. nicht valide sind, wird statt eines Pseudonyms ein Fehler-Parameter (error-Parameter) mit der Fehlerbeschreibung zurückgeliefert.

Ist der Request gänzlich ungültig, wird einer der folgenden HTTP Statuscodes in Verbindung mit einer OperationOutcome-Ressource zurückgegeben:
* 400: Fehlende oder fehlerhafte Parameter.
* 401: Fehlende Authentifizierung oder Autorisierung.
* 404: Parameter mit unbekanntem Inhalt.
* 422: Fehlende oder falsche Patienten-Attribute.

#### Beispiel

* [Request-Body](Parameters-Parameters-RequestPsnWorkflow-request-example-1.html)
* [Rückmeldung](Parameters-Parameters-RequestPsnWorkflow-response-example-1.html)
