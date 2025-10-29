# ConsentPolicyClass - v2025.1.0



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "ConsentPolicyClassCS",
  "url" : "https://ths-greifswald.de/fhir/CodeSystem/gics/ConsentPolicyClass",
  "version" : "2025.1.0",
  "name" : "ConsentPolicyClass",
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
  "description" : "Extensible description of the application perspective of a ConsentPolicy (e.g. selected data view 'IDAT')",
  "purpose" : "First axis 'Class' of the 'Semantic Consent Code (SCC)' for use as Consent.provision.class",
  "copyright" : "Copyright 2020-2025 Unabhängige Treuhandstelle der Universitätsmedizin Greifswald",
  "caseSensitive" : true,
  "content" : "complete",
  "count" : 15,
  "concept" : [
    {
      "code" : "BIOMAT",
      "display" : "BIOMAT",
      "designation" : [
        {
          "language" : "de-DE",
          "value" : "Biomaterialien"
        },
        {
          "language" : "en-UK",
          "value" : "biosamples"
        }
      ]
    },
    {
      "code" : "BIOMAT_analysed_data",
      "display" : "BIOMAT_analysed_data",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Auf Biomaterialien basierende Analysedaten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "BIOMAT_Analysedaten"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "analysed data based on biosamples"
        }
      ]
    },
    {
      "code" : "BIOMAT_retrospective",
      "display" : "BIOMAT_retrospective",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Retrospektive Biomaterialien"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "BIOMAT_retrospektiv"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "retrospective biosamples"
        }
      ]
    },
    {
      "code" : "BIOMAT_analysed_data_retrospective",
      "display" : "BIOMAT_analysed_data_retrospective",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Auf retrospektiven Biomaterialien basierende Analysedaten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "BIOMAT_Analysedaten_retrospektiv"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "analysed data based on retrospective biosamples"
        }
      ]
    },
    {
      "code" : "BIOMAT_additional_sampling",
      "display" : "BIOMAT_additional_sampling",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Biomaterialien, insbesondere zusätzlicher Mengen"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "BIOMAT_Zusatzmengen"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "biosamples, specifically additional sampling"
        }
      ]
    },
    {
      "code" : "PII",
      "display" : "PII",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Personenidentifizierende Daten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "IDAT"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "personal identifying information"
        }
      ]
    },
    {
      "code" : "IMGDAT",
      "display" : "IMGDAT",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Bilder und Bilddaten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "IMGDAT"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "images and image data"
        }
      ]
    },
    {
      "code" : "HIDAT",
      "display" : "HIDAT",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Krankenkassendaten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "KDAT"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "health insurance data"
        }
      ]
    },
    {
      "code" : "HIDAT_HIPN",
      "display" : "HIDAT_HIPN",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Krankenkassendaten, insbesondere die Krankenkassenversichertennummer"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "KDAT_KVNR"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "health insurance data, specifically the health insurance member ID or policy number"
        }
      ]
    },
    {
      "code" : "HIDAT_retrospective",
      "display" : "HIDAT_retrospective",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Retrospektive Krankenkassendaten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "KDAT_retrospektiv"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "retrospective health insurance data"
        }
      ]
    },
    {
      "code" : "MDAT",
      "display" : "MDAT",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Medizinische Daten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "MDAT"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "medical data"
        }
      ]
    },
    {
      "code" : "MDAT_GECCO83",
      "display" : "MDAT_GECCO83",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Medizinische Daten, insbesondere GECCO83 Datensatz"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "MDAT_GECCO83"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "medical data, specifically the GECCO83 data set"
        }
      ]
    },
    {
      "code" : "MDAT_retrospective",
      "display" : "MDAT_retrospective",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Retrospektive medizinische Daten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "MDAT_retrospektiv"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "retrospective medical data"
        }
      ]
    },
    {
      "code" : "BIOMAT_metadata",
      "display" : "BIOMAT_metadata",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Biomaterialien-spezifische Metadaten wie zum Beispiel zu Lagerung und Prozessierung"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "BIOMAT_Metadaten"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "metadata regarding biosamples such as storage and processing"
        }
      ]
    },
    {
      "code" : "PIDAT",
      "display" : "PIDAT",
      "designation" : [
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "Rentenversicherungsdaten"
        },
        {
          "language" : "de-DE",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000013009"
          },
          "value" : "PIDAT"
        },
        {
          "language" : "en-UK",
          "use" : {
            "system" : "http://snomed.info/sct",
            "code" : "900000000000003001"
          },
          "value" : "pension insurance data"
        }
      ]
    }
  ]
}

```
