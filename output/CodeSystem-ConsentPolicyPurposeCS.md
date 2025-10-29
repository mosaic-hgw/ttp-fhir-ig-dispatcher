# ConsentPolicyPurpose - v2025.1.0



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "ConsentPolicyPurposeCS",
  "url" : "https://ths-greifswald.de/fhir/CodeSystem/gics/ConsentPolicyPurpose",
  "version" : "2025.1.0",
  "name" : "ConsentPolicyPurpose",
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
  "description" : "Expandable specification of the application context and/or scope of a consent policy or module",
  "purpose" : "Third axis 'purpose' of the 'Semantic Consent Code (SCC)' for use as Consent.provision.purpose",
  "copyright" : "Copyright 2020-2025 Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "caseSensitive" : true,
  "content" : "complete",
  "count" : 33,
  "concept" : [
    {
      "code" : "health_state",
      "display" : "health_state",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "des Gesundheitszustandes"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Gesundheitszustand"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "the state of health"
        }
      ]
    },
    {
      "code" : "general_practitioner",
      "display" : "general_practitioner",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "des Hausarztes"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Arzt"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "from/to the general practitioner /family doctor"
        }
      ]
    },
    {
      "code" : "physician",
      "display" : "physician",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "des Arztes"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Hausarzt"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "from/to the physician"
        }
      ]
    },
    {
      "code" : "CRO",
      "display" : "CRO",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "von/an eine Contract Research Organisation und oder eine klinische Koordinierungsstelle (KKS)"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "CRO"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "from/to a clinical research organisation"
        }
      ]
    },
    {
      "code" : "third_parties",
      "display" : "third_parties",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "von/an/mit Dritte(n) Forschungspartner(n)"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Dritte"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "from/to third parties /with third party research partner(s)"
        }
      ]
    },
    {
      "code" : "EU_GDPR_LEVEL",
      "display" : "EU_GDPR_LEVEL",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "an Länder mit EU Datenschutzniveau"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "EU_DSGVO_NIVEAU"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "to countries with EU data protection level"
        }
      ]
    },
    {
      "code" : "non_EU_GDPR_LEVEL",
      "display" : "non_EU_GDPR_LEVEL",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "an Länder ohne EU Datenschutzniveau"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "non_EU_DSGVO_NIVEAU"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "to countries without EU data protection level"
        }
      ]
    },
    {
      "code" : "industry",
      "display" : "industry",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "an Partner aus dem Bereich der Industrie"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Industrie"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "to partners from the industrial sector"
        }
      ]
    },
    {
      "code" : "health_records",
      "display" : "health_records",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "durch Übertrag in/aus (elektronischen) Krankenunterlagen/Patientenakten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Krankenunterlagen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "by transfer to/from (electronic) health records"
        }
      ]
    },
    {
      "code" : "monitoring",
      "display" : "monitoring",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "im Rahmen eines Monitoring"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Monitoring"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "as part of a monitoring"
        }
      ]
    },
    {
      "code" : "non_profit",
      "display" : "non_profit",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "an Partner aus Non-Profit-Organisationen"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "non_profit"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "to partners from non-profit organisations"
        }
      ]
    },
    {
      "code" : "pharma",
      "display" : "pharma",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "an eine am Sponsoring beteiligte Pharmafirma"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "pharma"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "to a pharmaceutical company involved in the sponsorship"
        }
      ]
    },
    {
      "code" : "project_specific",
      "display" : "project_specific",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "im Rahmen des spezifischen Vorhabens/Projektes oder der spezifischen Studie"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Vorhaben_spezifisch"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "for a  specific research project or study"
        }
      ]
    },
    {
      "code" : "project_participation",
      "display" : "project_participation",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "über die Teilnahme der betroffenen Person am spezifischen Vorhaben/Projekt oder einer spezifischen Studie"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Vorhaben_Teilnahme"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "on the participation of the data subject in the specific project or a specific study"
        }
      ]
    },
    {
      "code" : "death",
      "display" : "death",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "im Falle des Todes der betroffenen Person"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Tod"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in the event of the death of the person concerned"
        }
      ]
    },
    {
      "code" : "timely_unrestricted",
      "display" : "timely_unrestricted ",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "ohne zeitliche Einschränkung"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "uneingeschraenkt"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : " without timely restriction"
        }
      ]
    },
    {
      "code" : "timely_restricted",
      "display" : "timely_restricted",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "mit zeitlicher Einschränkung"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "zeitlich_eingeschraenkt"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "with timely restriction"
        }
      ]
    },
    {
      "code" : "once",
      "display" : "once",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "einmalig"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "einmalig"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "once"
        }
      ]
    },
    {
      "code" : "databases",
      "display" : "databases",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Informationen anderer Datenbanken"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Datenbanken"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "information from other databases"
        }
      ]
    },
    {
      "code" : "additional_collection",
      "display" : "additional_collection",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Erhebung zusätzlicher [CLASS]"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "weitere_Erhebungen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "collection of additional [CLASS]"
        }
      ]
    },
    {
      "code" : "additional_studies",
      "display" : "additional_studies",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Informationen zu neuen Vorhaben/Projekten oder Studien"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "weitere_Studien"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "information on new projects or studies"
        }
      ]
    },
    {
      "code" : "additional_findings",
      "display" : "additional_findings",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Mitteilung von Zusatz- oder Nebenbefunden"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Zusatzbefund"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "notification of additional or incidental findings"
        }
      ]
    },
    {
      "code" : "HI",
      "display" : "HI",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "von/an Krankenversicherungen"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "KV"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "from/to health insurances"
        }
      ]
    },
    {
      "code" : "PI",
      "display" : "PI",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "von/an Rentenversicherungen"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "RV"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "from/to pension insurances"
        }
      ]
    },
    {
      "code" : "results",
      "display" : "results",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Mitteilung von Forschungsergebnissen"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Ergebnisse"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "communication of research results"
        }
      ]
    },
    {
      "code" : "significant",
      "display" : "significant",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "[PURPOSE] mit erheblicher Bedeutung"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Erhebliche_Bedeutung"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "[PURPOSE] with considerable significance"
        }
      ]
    },
    {
      "code" : "quality_assurance",
      "display" : "quality_assurance ",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "zu Zwecken der Qualitätssicherung"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "qualitaetssicherung"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "for quality assurance purposes"
        }
      ]
    },
    {
      "code" : "scientific",
      "display" : "scientific",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "im wissenschaftlichen Kontext"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "wissenschaftlich"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in a scientific context"
        }
      ]
    },
    {
      "code" : "highly_specific",
      "display" : "highly_specific",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in einer relevanten und hochspezifischen Weise"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "hochspezifisch"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in a relevant highly specific way"
        }
      ]
    },
    {
      "code" : "legally_based_registry",
      "display" : "legally_based_registry",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "im Rahmen eines Registers auf gesetzlicher Grundlage"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "gesetzliches_register"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "within the framework of a register on a legal basis"
        }
      ]
    },
    {
      "code" : "laboratory",
      "display" : "laboratory",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in / aus einem Labor"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "Labor"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in a / of a laboratory"
        }
      ]
    },
    {
      "code" : "genetic",
      "display" : "genetic",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "genetisch"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "genetisch"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "genetic"
        }
      ]
    },
    {
      "code" : "authority",
      "display" : "authority",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in einer /von einer / durch eine Behörde"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "behörde"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "in / from / by an authority"
        }
      ]
    }
  ]
}

```
