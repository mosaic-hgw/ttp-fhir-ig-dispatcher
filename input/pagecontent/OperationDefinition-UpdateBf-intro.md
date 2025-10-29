#### Zweck
Aktualisierung eines bestehenden Bloomfilters (z.B. bei geänderter Konfiguration oder vorheriger fehlerhafter Übermittlung) bezogen auf ein bereits bekanntes Pseudonym.

<p align="center">
  <img width="700" src="assets/images/fhirgw-updateBf.png">
</p>

#### Voraussetzung
- API-Key: Der spezifizierte API-Key muss valide und zum Aufruf der Methode autorisiert sein. Der API-KEY wird im Request-Header übermittelt.
- Die spezifizierte Studie (study) muss im Zielsystem bekannt und angelegt sein.
- Die spezifizierte Quell-Domäne (source) muss im Zielsystem bekannt und angelegt sein.
- Das spezifizierte Pseudonym (pseudonym) muss im Zielsystem bekannt und angelegt sein.
