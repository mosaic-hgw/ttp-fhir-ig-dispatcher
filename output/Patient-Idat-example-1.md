# Idat-example-1 - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "Patient",
  "id" : "Idat-example-1",
  "meta" : {
    "profile" : [
      "https://ths-greifswald.de/fhir/StructureDefinition/dispatcher/Patient/Idat"
    ]
  },
  "extension" : [
    {
      "url" : "http://hl7.org/fhir/StructureDefinition/patient-birthPlace",
      "valueAddress" : {
        "city" : "Musterhausen"
      }
    },
    {
      "extension" : [
        {
          "url" : "code",
          "valueCodeableConcept" : {
            "coding" : [
              {
                "system" : "urn:iso:std:iso:3166",
                "code" : "DE"
              }
            ]
          }
        }
      ],
      "url" : "http://hl7.org/fhir/StructureDefinition/patient-nationality"
    }
  ],
  "name" : [
    {
      "family" : "Mustermann",
      "given" : ["Martin"],
      "prefix" : ["Dr. med."],
      "_prefix" : [
        {
          "extension" : [
            {
              "url" : "http://hl7.org/fhir/StructureDefinition/iso21090-EN-qualifier",
              "valueCode" : "AC"
            }
          ]
        }
      ]
    }
  ],
  "gender" : "male",
  "birthDate" : "1965-12-03"
}

```
