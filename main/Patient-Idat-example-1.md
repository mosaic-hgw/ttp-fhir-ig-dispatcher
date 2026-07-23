# Idat-example-1 - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Idat-example-1**

## Example Patient: Idat-example-1

Profile: [IDAT](StructureDefinition-Idat.md)

Martin Mustermann Male, DoB: 1965-12-03

-------

| | |
| :--- | :--- |
| Patient Nationality: | * code: Germany
 |
| [Patient Birth Place](http://hl7.org/fhir/extensions/5.3.0/StructureDefinition-patient-birthPlace.html) | Musterhausen |



## Resource Content

```json
{
  "resourceType" : "Patient",
  "id" : "Idat-example-1",
  "meta" : {
    "profile" : ["https://ths-greifswald.de/fhir/StructureDefinition/dispatcher/Patient/Idat"]
  },
  "extension" : [{
    "url" : "http://hl7.org/fhir/StructureDefinition/patient-birthPlace",
    "valueAddress" : {
      "city" : "Musterhausen"
    }
  },
  {
    "extension" : [{
      "url" : "code",
      "valueCodeableConcept" : {
        "coding" : [{
          "system" : "urn:iso:std:iso:3166",
          "code" : "DE"
        }]
      }
    }],
    "url" : "http://hl7.org/fhir/StructureDefinition/patient-nationality"
  }],
  "name" : [{
    "family" : "Mustermann",
    "given" : ["Martin"],
    "prefix" : ["Dr. med."],
    "_prefix" : [{
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/iso21090-EN-qualifier",
        "valueCode" : "AC"
      }]
    }]
  }],
  "gender" : "male",
  "birthDate" : "1965-12-03"
}

```
