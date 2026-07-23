# OperationOutcome-UpdateBf-response-example-1 - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **OperationOutcome-UpdateBf-response-example-1**

## Example OperationOutcome: OperationOutcome-UpdateBf-response-example-1

### Issues

| | | | | |
| :--- | :--- | :--- | :--- | :--- |
| - | **Severity** | **Code** | **Details** | **Diagnostics** |
| * | Information | Informational Note | existing resource updated | Bloomfilter updated. |



## Resource Content

```json
{
  "resourceType" : "OperationOutcome",
  "id" : "OperationOutcome-UpdateBf-response-example-1",
  "issue" : [{
    "severity" : "information",
    "code" : "informational",
    "details" : {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/operation-outcome",
        "code" : "MSG_UPDATED"
      }]
    },
    "diagnostics" : "Bloomfilter updated."
  }]
}

```
