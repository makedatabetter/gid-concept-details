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
			"id": "100392",
			"label": "Last-Name",
			"predictedColumns": 9,
			"confirmedColumns": 3,
			"eta": 4970728792,
			"coverage": 33.333333333333336,
			"impactArea": [{
				"id": "120001",
				"label": "GDPR"
			}, {
				"id": "120002",
				"label": "Credit Risk"
			}],
			"classificationAccuracyPercentage": 0.0,
			"exampleValues": [{
				"id": "3642043d",
				"label": "Breckell",
				"verified": "N"
			}, {
				"id": "ace70260",
				"label": "Pallister",
				"verified": "N"
			}, {
				"id": "0a0bdcae",
				"label": "Cleere",
				"verified": "N"
			}, {
				"id": "9430c213",
				"label": "Ruppertz",
				"verified": "N"
			}, {
				"id": "40653d98",
				"label": "Newcomen",
				"verified": "N"
			}, {
				"id": "3ecdaab9",
				"label": "Mulvenna",
				"verified": "N"
			}, {
				"id": "afacd702",
				"label": "Crutchley",
				"verified": "N"
			}, {
				"id": "9ed6b924",
				"label": "Smidmore",
				"verified": "N"
			}, {
				"id": "46f1198c",
				"label": "Baynes",
				"verified": "N"
			}, {
				"id": "68144aa9",
				"label": "Sterzaker",
				"verified": "N"
			}, {
				"id": "03d4b129",
				"label": "Echallier",
				"verified": "N"
			}, {
				"id": "e0a61327",
				"label": "Corps",
				"verified": "N"
			}, {
				"id": "f21512c4",
				"label": "Orrom",
				"verified": "N"
			}, {
				"id": "427b01d1",
				"label": "Sylvester",
				"verified": "N"
			}, {
				"id": "e9a03cbc",
				"label": "Vidineev",
				"verified": "N"
			}, {
				"id": "5450481e",
				"label": "Ellinor",
				"verified": "N"
			}, {
				"id": "fc56d55e",
				"label": "Karpman",
				"verified": "N"
			}, {
				"id": "ad0e463b",
				"label": "Berzons",
				"verified": "N"
			}, {
				"id": "94aceefd",
				"label": "Danshin",
				"verified": "N"
			}, {
				"id": "2b24a83f",
				"label": "Christensen",
				"verified": "N"
			}, {
				"id": "845ce769",
				"label": "McKinstry",
				"verified": "N"
			}, {
				"id": "12d7588c",
				"label": "Knibb",
				"verified": "N"
			}, {
				"id": "16a47b3e",
				"label": "Bassindale",
				"verified": "N"
			}, {
				"id": "b6aed81a",
				"label": "Donaher",
				"verified": "N"
			}, {
				"id": "4cba59ba",
				"label": "Conti",
				"verified": "N"
			}, {
				"id": "edf4c548",
				"label": "Gentzsch",
				"verified": "N"
			}, {
				"id": "a8243e82",
				"label": "Geldeard",
				"verified": "N"
			}, {
				"id": "ec9f7c38",
				"label": "Somerlie",
				"verified": "N"
			}, {
				"id": "c360f7ef",
				"label": "Flea",
				"verified": "N"
			}, {
				"id": "f20df0f3",
				"label": "Dilland",
				"verified": "N"
			}],
			"patterns": [{
				"id": "600408",
				"label": "Zzzzzzz",
				"verified": "N",
				"count": 23
			}, {
				"id": "600405",
				"label": "Zzzzz",
				"verified": "N",
				"count": 14
			}, {
				"id": "600401",
				"label": "Zzzzzz",
				"verified": "N",
				"count": 11
			}, {
				"id": "600406",
				"label": "Zzzzzzzz-Zzzzzz",
				"verified": "N",
				"count": 1
			}, {
				"id": "600399",
				"label": "Zzzzzzzz",
				"verified": "N",
				"count": 25
			}, {
				"id": "600407",
				"label": "Zzzz",
				"verified": "N",
				"count": 8
			}, {
				"id": "600403",
				"label": "Zzzzzzzzzzzz",
				"verified": "N",
				"count": 1
			}, {
				"id": "600409",
				"label": "Zzz",
				"verified": "N",
				"count": 1
			}, {
				"id": "600404",
				"label": "Zzzzzzzzzz",
				"verified": "N",
				"count": 3
			}, {
				"id": "600400",
				"label": "Zzzzzzzzzzz",
				"verified": "N",
				"count": 1
			}, {
				"id": "600402",
				"label": "ZzZzzzzzz",
				"verified": "N",
				"count": 1
			}, {
				"id": "600410",
				"label": "Zzzzzzzzz",
				"verified": "N",
				"count": 13
			}],
			"synonyms": [{
				"id": "700132",
				"label": "cust_name",
				"verified": "N",
				"relevance": 27.0
			}, {
				"id": "700136",
				"label": "cust_id",
				"verified": "N",
				"relevance": 55.00000000000001
			}, {
				"id": "700125",
				"label": "user_name",
				"verified": "N",
				"relevance": 11.0
			}, {
				"id": "700131",
				"label": "f_name",
				"verified": "N",
				"relevance": 11.0
			}, {
				"id": "700127",
				"label": "last_name",
				"verified": "N",
				"relevance": 20.0
			}, {
				"id": "700134",
				"label": "first_name",
				"verified": "N",
				"relevance": 22.0
			}, {
				"id": "700133",
				"label": "customer_name",
				"verified": "N",
				"relevance": 11.0
			}, {
				"id": "700126",
				"label": "l_name",
				"verified": "N",
				"relevance": 11.0
			}, {
				"id": "700135",
				"label": "cust_phone",
				"verified": "N",
				"relevance": 9.0
			}, {
				"id": "700130",
				"label": "cust_fname",
				"verified": "N",
				"relevance": 9.0
			}],
			"exampleColumns": [{
				"id": "e2c8f630-4a37-38d7-9359-1d1be8375fcd",
				"label": "l_name",
				"verified": "N",
				"relevance": 1.0
			}, {
				"id": "28389982-3cdc-30d6-bc3f-cec02ae547ff",
				"label": "last_name",
				"verified": "N",
				"relevance": 1.0
			}, {
				"id": "8eefd496-038d-3485-9b32-3eece55d3569",
				"label": "last_name",
				"verified": "N",
				"relevance": 1.0
			}, {
				"id": "4ed34e05-5aa8-3e24-b17f-b57305156ad9",
				"label": "cust_lname",
				"verified": "N",
				"relevance": 1.0
			}, {
				"id": "4ed34e05-5aa8-3e24-b17f-b57305156ad9",
				"label": "cust_lname",
				"verified": "N",
				"relevance": 1.0
			}],
			"relatedConcepts": [{
				"id": "100376",
				"label": "Email-Address",
				"relevance": 18.0
			}, {
				"id": "100358",
				"label": "Birth-Date",
				"relevance": 16.0
			}, {
				"id": "100352",
				"label": "Address",
				"relevance": 12.0
			}, {
				"id": "100386",
				"label": "First-Name",
				"relevance": 18.0
			}, {
				"id": "100033",
				"label": "City",
				"relevance": 2.0
			}, {
				"id": "100387",
				"label": "Gender",
				"relevance": 17.0
			}, {
				"id": "100501",
				"label": "person-id",
				"relevance": 17.0
			}],
			"applications": [{
				"id": "100034",
				"label": "Billing and Collections"
			}, {
				"id": "100003",
				"label": "Advanced Information Services"
			}]
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