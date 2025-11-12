# ConsentStatusWithdrawalShortValues - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "ConsentStatusWithdrawalShortValuesVS",
  "url" : "https://ths-greifswald.de/fhir/ValueSet/gics/ConsentStatusWithdrawalShortValues",
  "version" : "2025.2.0",
  "name" : "ConsentStatusWithdrawalShortValues",
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
        "system" : "https://ths-greifswald.de/fhir/CodeSystem/gics/ConsentStatus",
        "concept" : [
          {
            "code" : "WITHDRAWN"
          },
          {
            "code" : "NOT_CHOSEN"
          }
        ]
      }
    ]
  }
}

```
