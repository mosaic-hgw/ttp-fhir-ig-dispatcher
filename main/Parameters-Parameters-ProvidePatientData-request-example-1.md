# Parameters-ProvidePatientData-request-example-1 - v2025.2.0

 ![](assets/images/Design-Logo-THS-deutsch-271-padding.png) 

 
 2025.2.0 - ci-build  

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Parameters-ProvidePatientData-request-example-1**

## Example Parameters: Parameters-ProvidePatientData-request-example-1



## Resource Content

```json
{
  "resourceType" : "Parameters",
  "id" : "Parameters-ProvidePatientData-request-example-1",
  "parameter" : [{
    "name" : "taskId",
    "valueId" : "064ddebf-b20e-468a-97fd-88097bcdbc11"
  },
  {
    "name" : "target",
    "valueString" : "eyematics"
  },
  {
    "name" : "patient",
    "resource" : {
      "resourceType" : "Patient",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/patient-birthPlace",
        "valueAddress" : {
          "city" : "Musterhausen"
        }
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
  }]
}

```
