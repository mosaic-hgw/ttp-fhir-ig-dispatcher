# PseudonymizePatient-Bundle-response-example-1 - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **PseudonymizePatient-Bundle-response-example-1**

## Example Bundle: PseudonymizePatient-Bundle-response-example-1



## Resource Content

```json
{
  "resourceType" : "Bundle",
  "id" : "PseudonymizePatient-Bundle-response-example-1",
  "type" : "batch-response",
  "entry" : [{
    "resource" : {
      "resourceType" : "Parameters",
      "id" : "PseudonymizePatient-Bundle-response-example-1-Par1",
      "parameter" : [{
        "name" : "externalPatientId",
        "valueId" : "aaaaaaaa-8a1e-4442-af99-50abc27d6f52"
      },
      {
        "name" : "pseudonym",
        "part" : [{
          "name" : "target",
          "valueIdentifier" : {
            "system" : "http://my.fhir.domain.local/fhir/sid/domains",
            "value" : "MyStudy-Domain1"
          }
        },
        {
          "name" : "value",
          "valueIdentifier" : {
            "system" : "http://my.fhir.domain.local/fhir/sid/pseudonyms",
            "value" : "56464986521"
          }
        }]
      },
      {
        "name" : "pseudonym",
        "part" : [{
          "name" : "target",
          "valueIdentifier" : {
            "system" : "http://my.fhir.domain.local/fhir/sid/domains",
            "value" : "MyStudy-Domain2"
          }
        },
        {
          "name" : "value",
          "valueIdentifier" : {
            "system" : "http://my.fhir.domain.local/fhir/sid/pseudonyms",
            "value" : "8976834765347"
          }
        }]
      }]
    },
    "response" : {
      "status" : "200",
      "outcome" : {
        "resourceType" : "OperationOutcome",
        "id" : "PseudonymizePatient-Bundle-response-example-1-Par1OpO",
        "issue" : [{
          "severity" : "information",
          "code" : "informational",
          "diagnostics" : "Operation completed successfully."
        }]
      }
    }
  },
  {
    "resource" : {
      "resourceType" : "Parameters",
      "id" : "PseudonymizePatient-Bundle-response-example-1-Par2",
      "parameter" : [{
        "name" : "externalPatientId",
        "valueId" : "bbbbbbbb-e258-4471-9ac3-6dfdfac35a6e"
      },
      {
        "name" : "pseudonym",
        "part" : [{
          "name" : "target",
          "valueIdentifier" : {
            "system" : "http://my.fhir.domain.local/fhir/sid/domains",
            "value" : "MyStudy-Domain15"
          }
        },
        {
          "name" : "value",
          "valueIdentifier" : {
            "system" : "http://my.fhir.domain.local/fhir/sid/pseudonyms",
            "value" : "8976834765347"
          }
        }]
      }]
    },
    "response" : {
      "status" : "404",
      "outcome" : {
        "resourceType" : "OperationOutcome",
        "id" : "PseudonymizePatient-Bundle-response-example-1-Par2OpO",
        "issue" : [{
          "severity" : "fatal",
          "code" : "security",
          "diagnostics" : "Target domain 'NotMyStudy-Domain15' not found."
        }]
      }
    }
  }]
}

```
