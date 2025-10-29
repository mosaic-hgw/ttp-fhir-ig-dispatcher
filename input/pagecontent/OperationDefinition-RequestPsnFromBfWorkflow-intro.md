#### Zweck
Anlegen und Matching von Patienten rein auf Basis von Bloomfiltern (PPRL) für einen gegebenen Geltungsbereich (Studie und Standort). Rückgabe der generierten Pseudonyme (z.b. DIC-PSN(s)) als Parameter.

<p align="center">
  <img width="700" src="assets/images/fhirgw-requestpsnbfworkflow.png">
</p>

#### Voraussetzung
- API-Key: Der spezifizierte API-Key muss valide und zum Aufruf der Methode autorisiert sein. Der API-KEY wird im Request-Header übermittelt.
- Die spezifizierte Studie muss im Zielsystem bekannt und angelegt sein.
- Die übermittelten Bloomfilter müssen valide sein.
- Die standortspezifische Domäne (target) muss im Zielsystem bekannt und angelegt sein.
