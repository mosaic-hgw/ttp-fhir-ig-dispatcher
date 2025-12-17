# IDAT - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "Idat",
  "url" : "https://ths-greifswald.de/fhir/StructureDefinition/dispatcher/Patient/Idat",
  "version" : "2025.2.0",
  "name" : "Idat",
  "title" : "IDAT",
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
  "description" : "Patienten-Profil zur Übermittlung von angeforderten IDAT an die fTTP für den Clearing-Prozess.",
  "copyright" : "Copyright 2020-2025 Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    },
    {
      "identity" : "cda",
      "uri" : "http://hl7.org/v3/cda",
      "name" : "CDA (R2)"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    },
    {
      "identity" : "loinc",
      "uri" : "http://loinc.org",
      "name" : "LOINC code for the element"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Patient",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Patient",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Patient",
        "path" : "Patient",
        "short" : "Patienten-Profil zur Übermittlung von angeforderten IDAT",
        "comment" : "Die per $requestTasks vorgegebenen Element-Bezeichner sind wie folgt gemappt:\r\n\r\ngiven: name.given\r\nfamily: name.family (mit name.use!='maiden' oder nicht vorhanden)\r\nprefix: name.prefix\r\nsuffix: name.suffix\r\nbirthdate: birthDate\r\ngender: gender\r\naddress-line: address.line\r\naddress-city: address.city\r\naddress-postalcode: address.postalCode\r\nbirthplace: extension('http://hl7.org/fhir/StructureDefinition/patient-birthPlace').city\r\nmaidenname: name.family (mit name.use='maiden')\r\ndegree: name.prefix (ggf. mit gesetzter Extension http://hl7.org/fhir/StructureDefinition/iso21090-EN-qualifier mit Code 'AC')\r\nlanguage: communication.language (mit communication.preferred=true)\r\nnationality: extension(http://hl7.org/fhir/StructureDefinition/patient-nationality).valueCode.coding.code oder extension(http://hl7.org/fhir/StructureDefinition/patient-nationality).valueCode.textextension(http://hl7.org/fhir/StructureDefinition/patient-nationality).code.text\r\nmaritalstatus: maritalStatus.coding.code oder maritalStatus.text"
      },
      {
        "id" : "Patient.extension",
        "path" : "Patient.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        }
      },
      {
        "id" : "Patient.extension:birthPlace",
        "path" : "Patient.extension",
        "sliceName" : "birthPlace",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://hl7.org/fhir/StructureDefinition/patient-birthPlace"]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Patient.extension:birthPlace.value[x]",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x]",
        "mustSupport" : true
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].use",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].use",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].type",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].type",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].text",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].text",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].line",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].line",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].city",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].city",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].district",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].district",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].state",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].state",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].postalCode",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].postalCode",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].country",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.value[x].country",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:birthPlace.value[x].period",
        "path" : "Patient.extension.value[x].period",
        "max" : "0"
      },
      {
        "id" : "Patient.extension:nationality",
        "path" : "Patient.extension",
        "sliceName" : "nationality",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://hl7.org/fhir/StructureDefinition/patient-nationality"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Patient.extension:nationality.extension:code",
        "path" : "Patient.extension.extension",
        "sliceName" : "code"
      },
      {
        "id" : "Patient.extension:nationality.extension:code.value[x]",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.extension.value[x]",
        "mustSupport" : true,
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://hl7.org/fhir/ValueSet/iso3166-1-2"
        }
      },
      {
        "id" : "Patient.extension:nationality.extension:code.value[x].coding",
        "path" : "Patient.extension.extension.value[x].coding",
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Patient.extension:nationality.extension:code.value[x].coding.system",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.extension.value[x].coding.system",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.extension:nationality.extension:code.value[x].coding.code",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.extension.value[x].coding.code",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.extension:nationality.extension:code.value[x].text",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-translatable",
            "valueBoolean" : true
          },
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.extension.extension.value[x].text",
        "mustSupport" : true
      },
      {
        "id" : "Patient.identifier",
        "path" : "Patient.identifier",
        "max" : "0"
      },
      {
        "id" : "Patient.active",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.active",
        "max" : "0"
      },
      {
        "id" : "Patient.name",
        "path" : "Patient.name",
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.use",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.name.use",
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.text",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.name.text",
        "max" : "0"
      },
      {
        "id" : "Patient.name.family",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.name.family",
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.given",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.name.given",
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.prefix",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.name.prefix",
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.prefix.extension",
        "path" : "Patient.name.prefix.extension",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "url"
            }
          ],
          "ordered" : false,
          "rules" : "open"
        }
      },
      {
        "id" : "Patient.name.prefix.extension:academic",
        "path" : "Patient.name.prefix.extension",
        "sliceName" : "academic",
        "min" : 0,
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://hl7.org/fhir/StructureDefinition/iso21090-EN-qualifier"
            ]
          }
        ],
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.prefix.extension:academic.value[x]",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.name.prefix.extension.value[x]",
        "fixedCode" : "AC",
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.suffix",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.name.suffix",
        "mustSupport" : true
      },
      {
        "id" : "Patient.name.period",
        "path" : "Patient.name.period",
        "max" : "0"
      },
      {
        "id" : "Patient.telecom",
        "path" : "Patient.telecom",
        "max" : "0"
      },
      {
        "id" : "Patient.gender",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.gender",
        "mustSupport" : true
      },
      {
        "id" : "Patient.birthDate",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.birthDate",
        "mustSupport" : true
      },
      {
        "id" : "Patient.deceased[x]",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.deceased[x]",
        "max" : "0"
      },
      {
        "id" : "Patient.address",
        "path" : "Patient.address",
        "mustSupport" : true
      },
      {
        "id" : "Patient.address.text",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.address.text",
        "max" : "0"
      },
      {
        "id" : "Patient.address.line",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.address.line",
        "mustSupport" : true
      },
      {
        "id" : "Patient.address.city",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.address.city",
        "mustSupport" : true
      },
      {
        "id" : "Patient.address.district",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.address.district",
        "max" : "0"
      },
      {
        "id" : "Patient.address.state",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.address.state",
        "max" : "0"
      },
      {
        "id" : "Patient.address.postalCode",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.address.postalCode",
        "mustSupport" : true
      },
      {
        "id" : "Patient.address.country",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.address.country",
        "max" : "0"
      },
      {
        "id" : "Patient.address.period",
        "path" : "Patient.address.period",
        "max" : "0"
      },
      {
        "id" : "Patient.maritalStatus",
        "path" : "Patient.maritalStatus",
        "mustSupport" : true,
        "binding" : {
          "extension" : [
            {
              "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-bindingName",
              "valueString" : "MaritalStatus"
            },
            {
              "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-isCommonBinding",
              "valueBoolean" : true
            }
          ],
          "strength" : "required",
          "description" : "The domestic partnership status of a person.",
          "valueSet" : "http://hl7.org/fhir/ValueSet/marital-status"
        }
      },
      {
        "id" : "Patient.maritalStatus.coding",
        "path" : "Patient.maritalStatus.coding",
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Patient.maritalStatus.coding.system",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.maritalStatus.coding.system",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.maritalStatus.coding.code",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.maritalStatus.coding.code",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.maritalStatus.text",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-translatable",
            "valueBoolean" : true
          },
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.maritalStatus.text",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.multipleBirth[x]",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.multipleBirth[x]",
        "max" : "0"
      },
      {
        "id" : "Patient.photo",
        "path" : "Patient.photo",
        "max" : "0"
      },
      {
        "id" : "Patient.contact",
        "path" : "Patient.contact",
        "max" : "0"
      },
      {
        "id" : "Patient.communication",
        "path" : "Patient.communication",
        "mustSupport" : true
      },
      {
        "id" : "Patient.communication.language",
        "path" : "Patient.communication.language",
        "mustSupport" : true,
        "binding" : {
          "extension" : [
            {
              "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-maxValueSet",
              "valueCanonical" : "http://hl7.org/fhir/ValueSet/all-languages"
            },
            {
              "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-bindingName",
              "valueString" : "Language"
            },
            {
              "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-isCommonBinding",
              "valueBoolean" : true
            }
          ],
          "strength" : "required",
          "description" : "A human language.",
          "valueSet" : "http://hl7.org/fhir/ValueSet/languages"
        }
      },
      {
        "id" : "Patient.communication.language.coding",
        "path" : "Patient.communication.language.coding",
        "max" : "1",
        "mustSupport" : true
      },
      {
        "id" : "Patient.communication.language.coding.system",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.communication.language.coding.system",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.communication.language.coding.code",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.communication.language.coding.code",
        "min" : 1,
        "mustSupport" : true
      },
      {
        "id" : "Patient.communication.language.text",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-translatable",
            "valueBoolean" : true
          },
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.communication.language.text",
        "mustSupport" : true
      },
      {
        "id" : "Patient.communication.preferred",
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
            "valueCode" : "normative"
          }
        ],
        "path" : "Patient.communication.preferred",
        "min" : 1,
        "fixedBoolean" : true,
        "mustSupport" : true
      },
      {
        "id" : "Patient.generalPractitioner",
        "path" : "Patient.generalPractitioner",
        "max" : "0"
      },
      {
        "id" : "Patient.managingOrganization",
        "path" : "Patient.managingOrganization",
        "max" : "0"
      },
      {
        "id" : "Patient.link",
        "path" : "Patient.link",
        "max" : "0"
      }
    ]
  }
}

```
