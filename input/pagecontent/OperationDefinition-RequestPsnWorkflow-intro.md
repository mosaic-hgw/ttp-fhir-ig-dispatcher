#### Zweck
Abfragen bzw. Anlegen von Pseudonymen auf Basis eines vorkonfigurierten Pseudonymisierungsablaufs (Workflow) für einen gegebenen Geltungsbereich (Studie und Standort).

Dabei wird stets ein oder mehrere Originalwerte einer Quell-Domäne in ein oder mehrere Pseudonyme der Ziel-Domäne pseudonymisiert. Ist der Originalwert bereits bekannt, wird das bereits zuvor generierte Pseudonym der Ziel-Domäne geliefert.

Diese Methode überführt Pseudonyme einer Stufe in eine andere Stufe. Dabei werden entweder bekannte Pseudonyme zurückgeliefert (Um-Pseudonymisierung) oder neue Pseudonyme generiert (Dritt-Pseudonymisierung).

Die Rückgabe der generierten standort- und studienspezifischen Pseudonyme erfolgt als Parameter.

<p align="center">
  <img width="700" src="assets/images/fhirgw-requestpsnworkflow.png">
</p>

#### Voraussetzung
- API-Key: Der spezifizierte API-Key muss valide und zum Aufruf der Methode autorisiert sein. Der API-KEY wird im Request-Header übermittelt.
- Die spezifizierte Studie muss im Zielsystem bekannt und angelegt sein.
- Die spezifizierte Quell-Domäne (source) muss im Zielsystem bekannt und angelegt sein.
- Die standortspezifische Domäne (target) muss im Zielsystem bekannt und angelegt sein.
- Das angegebene Event muss bekannt sein und der API-Key dafür autorisiert sein.
