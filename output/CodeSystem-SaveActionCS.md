# SaveAction - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "SaveActionCS",
  "url" : "https://ths-greifswald.de/fhir/CodeSystem/epix/SaveAction",
  "version" : "2025.2.0",
  "name" : "SaveAction",
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
  "description" : "Possible save actions in the context of adding patient identities.",
  "copyright" : "Copyright 2020-2025 Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "caseSensitive" : true,
  "content" : "complete",
  "count" : 4,
  "concept" : [
    {
      "code" : "DONT_SAVE",
      "display" : "don't save"
    },
    {
      "code" : "DONT_SAVE_ON_PERFECT_MATCH",
      "display" : "don't save on perfect match"
    },
    {
      "code" : "DONT_SAVE_ON_PERFECT_MATCH_EXCEPT_CONTACTS",
      "display" : "don't save on perfect match except contacts"
    },
    {
      "code" : "SAVE_ALL",
      "display" : "save all"
    }
  ]
}

```
