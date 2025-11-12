# ConsentPolicyAction - v2025.2.0



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "ConsentPolicyActionCS",
  "url" : "https://ths-greifswald.de/fhir/CodeSystem/gics/ConsentPolicyAction",
  "version" : "2025.2.0",
  "name" : "ConsentPolicyAction",
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
  "description" : "Extensible description of the permissible (data processing-) action resulting from consented module or policy.",
  "purpose" : "Second axis 'action' of the 'Semantic Consent Code (SCC)' for use as Consent.provision.action",
  "copyright" : "Copyright 2020-2025 Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "caseSensitive" : true,
  "content" : "complete",
  "count" : 14,
  "concept" : [
    {
      "code" : "provide",
      "display" : "provide",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Weitergabe von [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "bereitstellen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "transfer of [CLASS]"
        }
      ]
    },
    {
      "code" : "transfer_ownership",
      "display" : "transfer_ownership",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Übertragung des Eigentums an [CLASS] vom Teilnehmer an den Verantwortlichen/Datenverarbeiter/Träger der Biobank"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "uebertragen_eigentum"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "transfer the ownership of [CLASS] from the participant to the controller/data processor/carrier of the biobank."
        }
      ]
    },
    {
      "code" : "view",
      "display" : "view",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Einsicht in [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "einsehen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "insight into [CLASS]"
        }
      ]
    },
    {
      "code" : "collect",
      "display" : "collect",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Erhebung neuer [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "entnehmen; erheben"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "collection of new [CLASS]"
        }
      ]
    },
    {
      "code" : "analyse_genetic",
      "display" : "analyse_genetic",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Gewinnung von genetischen Daten aus [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "analysieren_genetisch"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "obtaining genetic data from [CLASS]"
        }
      ]
    },
    {
      "code" : "inform",
      "display" : "inform",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Information"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "informieren"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "information "
        }
      ]
    },
    {
      "code" : "store_process",
      "display" : "store_process",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Speicherung und Verarbeitung von [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "lagern_verarbeiten; speichern_verarbeiten"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "storage and processing of [CLASS]"
        }
      ]
    },
    {
      "code" : "contact",
      "display" : "contact",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Rekontaktierung des Teilnehmers (ggf. in Bezug auf [TAETIGKEIT|KONTEXT])"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "rekontaktieren"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "contact participant (if necessary, regarding [ACTIVITY|KONTEXT])"
        }
      ]
    },
    {
      "code" : "use",
      "display" : "use",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Bereitstellung von [CLASS] für Nutzung / Analysen / zu Auswertezwecken [PURPOSE]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "nutzen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "provision of [CLASS] for use / analyses / for evaluation purposes [PURPOSE]."
        }
      ]
    },
    {
      "code" : "process",
      "display" : "process",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Verarbeitung von [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "verarbeiten"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "processing of [CLASS]"
        }
      ]
    },
    {
      "code" : "merge",
      "display" : "merge",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Zusammenführung und ggf. überführen von [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "zusammenfuehren"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "merging and, if necessary, transferring of [CLASS]"
        }
      ]
    },
    {
      "code" : "query",
      "display" : "query",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Abfrage von [PURPOSE]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "abfragen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "query with/from [PURPOSE]"
        }
      ]
    },
    {
      "code" : "supplement",
      "display" : "supplement",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Ergänzende / kompletttierende Erhebung zusätzlicher [CLASS] mit / aus [PURPOSE]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "ergaenzen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "supplementary / complementary collection of additional [CLASS] with / from [PURPOSE]."
        }
      ]
    },
    {
      "code" : "link",
      "display" : "link",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Verknüpfung von Daten der betroffenen Person mit [PURPOSE]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "verknuepfen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "linking data of the data subject to [PURPOSE]"
        }
      ]
    }
  ]
}

```
