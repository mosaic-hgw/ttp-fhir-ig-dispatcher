#### Zweck
Identifizierende Daten (IDAT) werden für einen Clearing-Prozess an
die fTTP übertragen. Die darin enthaltenen Attribute (z.B. Vorname, Nachname, usw.)
dienen für ein konventionelles Record Linkage und werden danach in der fTTP
unwiederbringlich gelöscht.

<p align="center">
  <img width="700" src="assets/images/fhirgw-providePatientData.png">
</p>

#### Voraussetzung
- API-Key: Der spezifizierte API-Key muss valide und zum Aufruf der Methode autorisiert sein. Der API-KEY wird im Request-Header übermittelt.
- Die übermittelten IDAT müssen valide sein.
- Die TaskId muss valide sein.
- Der Standort hat zuvor seine Tasks abgerufen (vgl. requestTasks) und eine Aufgabe "send-idat" zugewiesen bekommen haben.
