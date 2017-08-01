## gid-concept-details

A data component to get detailed information for a given concept and user id

    <gid-concept-details concept='1' user='1' entity = "CONCEPT-DETAILS" conceptdetails='{{conceptdetails}}'></<gid-concept-details>
    
The fields 'concept' and 'entity' are  mandatory.

If 'apiUrl' is not provided, then the component would fetch sample data from mock json.

API endpoint:

    GET /concepts/{id}
    
Input:
- User Id
- Concept Id
- Selected Synonyms, Patterns, Related Concepts, Example Values for pivoting

Sample Input: (Query params)

    GET /concepts/{id}?synonyms=100052,100053,100054&patterns=100152,100152,100152&relatedConcepts=100652&exampleValues=200652

Output:
- Key Metadata
- Concept Detail


The output of this components will be as follows:

    {
      "concept": {
        "id": "100462",
        "label": "FICO-Score",
        "owner": {
          "id": "111001",
          "label": "Angela"
        },
        "predictedColumns": 5,
        "confirmedColumns": 3,
        "eta": 0,
        "coverage": 0.001,
        "impactArea": [
          {
            "id": "120002",
            "label": "Credit Risk"
          },
          {
            "id": "120001",
            "label": "GDPR"
          }
        ],
        "classificationAccuracyPercentage": 5,
        "applications": [
          {
            "id": "100492",
            "label": "Universal Biller"
          },
          {
            "id": "100252",
            "label": "Supplier Management Program"
          }
        ],
        "synonyms": [
          {
            "id": "100052",
            "label": "DOB",
            "relevance": 45,
            "verified": "Y"
          },
          {
            "id": "100053",
            "label": "Birthday",
            "relevance": 65,
            "verified": "N"
          }
        ],
        "patterns": [
          {
            "id": "100152",
            "label": "DD/MM/YY",
            "relevance": 37,
            "verified": "F"
          },
          {
            "id": "100153",
            "label": "MM/YY/DD",
            "relevance": 54,
            "verified": "Y"
          }
        ],
        "relatedConcepts": [
          {
            "id": "100652",
            "label": "First Name",
            "relevance": 44,
            "verified": "Y"
          },
          {
            "id": "100653",
            "label": "Last Name",
            "relevance": 32,
            "verified": "Y"
          }
        ],
        "exampleValues": [
          {
            "id": "200652",
            "label": "21/03/2007",
            "relevance": 90,
            "verified": "Y"
          },
          {
            "id": "200653",
            "label": "08/07/2006",
            "relevance": 80,
            "verified": "Y"
          }
        ],
        "exampleColumns": [
          {
            "id": "300652",
            "label": "DOB",
            "relevance": 90,
            "verified": "Y"
          },
          {
            "id": "300653",
            "label": "BIRTH_DAY",
            "relevance": 80,
            "verified": "Y"
          },
          {
            "id": "300654",
            "label": "ORDER_DATE",
            "relevance": 50,
            "verified": "Y"
          }
        ]
      }
    }


## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.