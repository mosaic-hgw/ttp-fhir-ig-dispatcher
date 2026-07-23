# Parameters-RequestPsnFromBfWorkflow-response-example-1 - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Parameters-RequestPsnFromBfWorkflow-response-example-1**

## Example Parameters: Parameters-RequestPsnFromBfWorkflow-response-example-1



## Resource Content

```json
{
  "resourceType" : "Parameters",
  "id" : "Parameters-RequestPsnFromBfWorkflow-response-example-1",
  "parameter" : [{
    "name" : "pseudonym-bf",
    "part" : [{
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
    }]
  },
  {
    "name" : "error",
    "part" : [{
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
    }]
  }]
}

```
