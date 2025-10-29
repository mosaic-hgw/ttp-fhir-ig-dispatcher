#### Aufruf und Rückgabe

Im Kontext dieser Operation wird das [PatientPseudonymized-Profil](StructureDefinition-PatientPseudonymized.html) verwendet.

Bei count = 0 wird nur lesend zugegriffen und werden keine Pseudonyme erzeugt. 
Bei count > 1 ist die Konfiguration von Multi-Psn-Domänen erforderlich. In diesem Fall kann die Rückgabe mehrere Parameter mit dem Bezeichner pseudonym enthalten.

Im Fehlerfall wird eine OperationOutcome-Ressource mit entsprechenden Informationen zurückgegeben. Bei Verwendung innerhalb eines Batch-Bundles (siehe Beispiele) wird in der Batch-Response neben diesem OperationOutcome auch eine Parameters-Ressource zurückgegeben, die auf die betroffene PatientId sowie das Target verweist.

#### Beispiel

* [Request-Body](Bundle-PseudonymizePatient-Bundle-request-example-1.html)
* [Rückmeldung](Bundle-PseudonymizePatient-Bundle-response-example-1.html)
