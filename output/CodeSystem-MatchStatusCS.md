# MatchStatus - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "MatchStatusCS",
  "url" : "https://ths-greifswald.de/fhir/CodeSystem/epix/MatchStatus",
  "version" : "2025.2.0",
  "name" : "MatchStatus",
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
  "description" : "Possible match statuses in the context of adding patient identities.",
  "copyright" : "Copyright 2020-2025 Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "caseSensitive" : true,
  "content" : "complete",
  "count" : 8,
  "concept" : [
    {
      "code" : "EXTERNAL_MATCH",
      "display" : "external match"
    },
    {
      "code" : "MATCH",
      "display" : "match"
    },
    {
      "code" : "MATCH_ERROR",
      "display" : "match error"
    },
    {
      "code" : "MULTIPLE_MATCH",
      "display" : "multiple match"
    },
    {
      "code" : "NO_MATCH",
      "display" : "no match"
    },
    {
      "code" : "PERFECT_MATCH",
      "display" : "perfect match"
    },
    {
      "code" : "PERFECT_MATCH_WITH_UPDATE",
      "display" : "perfect match with update"
    },
    {
      "code" : "POSSIBLE_MATCH",
      "display" : "possible match"
    }
  ]
}

```
