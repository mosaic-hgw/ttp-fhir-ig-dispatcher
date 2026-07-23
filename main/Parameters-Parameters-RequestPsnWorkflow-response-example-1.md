# Parameters-RequestPsnWorkflow-response-example-1 - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Parameters-RequestPsnWorkflow-response-example-1**

## Example Parameters: Parameters-RequestPsnWorkflow-response-example-1



## Resource Content

```json
{
  "resourceType" : "Parameters",
  "id" : "Parameters-RequestPsnWorkflow-response-example-1",
  "parameter" : [{
    "name" : "pseudonym",
    "part" : [{
      "name" : "original",
      "valueIdentifier" : {
        "system" : "https://ths-greifswald.de/gpas",
        "value" : "dic_1H51T"
      }
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
        "value" : "eyematics_6348Q7"
      }
    }]
  },
  {
    "name" : "error",
    "part" : [{
      "name" : "original",
      "valueIdentifier" : {
        "system" : "https://ths-greifswald.de/gpas",
        "value" : "dic_2Q42E"
      }
    },
    {
      "name" : "target",
      "valueIdentifier" : {
        "system" : "https://ths-greifswald.de/gpas",
        "value" : "eyematics"
      }
    },
    {
      "name" : "error-code",
      "valueCoding" : {
        "system" : "http://hl7.org/fhir/issue-type",
        "code" : "not-found",
        "display" : "Not Found"
      }
    }]
  }]
}

```
