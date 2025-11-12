# Parameters-RequestTasks-response-example-1 - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "Parameters",
  "id" : "Parameters-RequestTasks-response-example-1",
  "parameter" : [
    {
      "name" : "dic_psn_available",
      "part" : [
        {
          "name" : "bloomfilter",
          "valueBase64Binary" : "SWNoIGJpbiBlaW4gQmxvb21maWx0ZXIuIFZlcnNwcm9jaGVuLg=="
        },
        {
          "name" : "target",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "eyematics"
          }
        },
        {
          "name" : "pseudonym",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "mii_6348Q7"
          }
        }
      ]
    },
    {
      "name" : "send_idat",
      "part" : [
        {
          "name" : "expires",
          "valueInstant" : "2021-05-28T13:00:00.00+02:00"
        },
        {
          "name" : "taskId",
          "valueId" : "064ddebf-b20e-468a-97fd-88097bcdbc11"
        },
        {
          "name" : "pseudonym",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "mii_1244Q2"
          }
        },
        {
          "name" : "element",
          "valueCoding" : {
            "system" : "https://ths-greifswald.de/fhir/CodeSystem/dispatcher/IdatElements",
            "code" : "given"
          }
        },
        {
          "name" : "element",
          "valueCoding" : {
            "system" : "https://ths-greifswald.de/fhir/CodeSystem/dispatcher/IdatElements",
            "code" : "family"
          }
        },
        {
          "name" : "element",
          "valueCoding" : {
            "system" : "https://ths-greifswald.de/fhir/CodeSystem/dispatcher/IdatElements",
            "code" : "birthdate"
          }
        },
        {
          "name" : "element",
          "valueCoding" : {
            "system" : "https://ths-greifswald.de/fhir/CodeSystem/dispatcher/IdatElements",
            "code" : "gender"
          }
        },
        {
          "name" : "element",
          "valueCoding" : {
            "system" : "https://ths-greifswald.de/fhir/CodeSystem/dispatcher/IdatElements",
            "code" : "birthplace"
          }
        },
        {
          "name" : "element",
          "valueCoding" : {
            "system" : "https://ths-greifswald.de/fhir/CodeSystem/dispatcher/IdatElements",
            "code" : "degree"
          }
        }
      ]
    },
    {
      "name" : "repeat_request",
      "part" : [
        {
          "name" : "study",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "mii"
          }
        },
        {
          "name" : "bloomfilter",
          "valueBase64Binary" : "SWNoIGJpbiBlaW4gQmxvb21maWx0ZXIuIFZlcnNwcm9jaGVuLg=="
        },
        {
          "name" : "target",
          "valueIdentifier" : {
            "system" : "https://ths-greifswald.de/gpas",
            "value" : "eyematics"
          }
        }
      ]
    }
  ]
}

```
