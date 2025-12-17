# PolicyStatus - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "PolicyStatusVS",
  "url" : "https://ths-greifswald.de/fhir/ValueSet/gics/PolicyStatus",
  "version" : "2025.2.0",
  "name" : "PolicyStatus",
  "status" : "active",
  "experimental" : false,
  "date" : "2025-06-12",
  "publisher" : "Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "contact" : [
    {
      "name" : "Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
      "telecom" : [
        {
          "system" : "url",
          "value" : "https://www.ths-greifswald.de/"
        }
      ]
    }
  ],
  "copyright" : "Copyright 2020-2025 Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "compose" : {
    "include" : [
      {
        "valueSet" : ["http://hl7.org/fhir/ValueSet/consent-provision-type"]
      },
      {
        "system" : "http://terminology.hl7.org/CodeSystem/v3-NullFlavor",
        "concept" : [
          {
            "code" : "UNK"
          }
        ]
      }
    ]
  }
}

```
