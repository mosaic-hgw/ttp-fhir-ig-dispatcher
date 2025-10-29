#### Zweck
Tasks sind Aufgaben, die ein Standort regelmäßig abruft
und abarbeitet. Dies umfasst beispielsweise die Auflösung eines Clearing-Prozesses,
wenn ein Privacy-Preserving Record Linkage zu einem uneindeutigem Ergebnis kam. Es
wird empfohlen, die Aufgaben regelmäßig (und mehrmals die Woche) abzurufen.
Andernfalls können uneindeutige Matches nicht aufgelöst werden und entsprechende
Pseudonyme nicht vergeben werden. Aufgaben können sein: Einen vorhergehenden
Request erneut senden, das Pseudonym nach einem Clearing-Prozess abrufen und am
Standort hinterlegen, Identifizierende Daten zu einem vorher gesendeten Bloomfilter
senden. Aufgaben haben ein Verfallsdatum. Werden diese nicht rechtzeitig abgearbeitet,
wird der auslösende Prozess abgebrochen (z.B. Clearing-Prozess).

<p align="center">
  <img width="700" src="assets/images/fhirgw-requestTasks.png">
</p>

#### Voraussetzung
- API-Key: Der spezifizierte API-Key muss valide und zum Aufruf der Methode autorisiert sein. Der API-KEY wird im Request-Header übermittelt.
- Die spezifizierte Studie muss im Zielsystem bekannt und angelegt sein.
- Die standortspezifische Ziel-Domäne (target) muss im Zielsystem bekannt und angelegt sein.
