# Parameters-RequestPsnFromBfWorkflow-response-example-1 - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "Parameters",
  "id" : "Parameters-RequestPsnFromBfWorkflow-response-example-1",
  "parameter" : [
    {
      "name" : "pseudonym-bf",
      "part" : [
        {
          "name" : "bloomfilter",
          "valueBase64Binary" : "SWNoIGJpbiBlaW4gQmxvb21maWx0ZXIuIFZlcnNwcm9jaGVuLg=="
        },
        {
          "name" : "target",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "dic_muenster"
          }
        },
        {
          "name" : "pseudonym",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "dic_1H51T"
          }
        }
      ]
    },
    {
      "name" : "error",
      "part" : [
        {
          "name" : "bloomfilter",
          "valueBase64Binary" : "ZHVtbXk="
        },
        {
          "name" : "target",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "dic_muenster"
          }
        },
        {
          "name" : "error-code",
          "valueCoding" : {
            "system" : "http://hl7.org/fhir/issue-type",
            "code" : "not-found",
            "display" : "Not Found"
          }
        }
      ]
    }
  ]
}

```
