{
  "info": {
    "name": "Attom Data Solutions API Returns lines of business categories.",
    "_postman_id": "1d75d83f-1703-4e9b-a98b-e1fc5fba6c4e",
    "description": "This lookup can be used to show the full list of Lines of Businesses (LOB), and which categories they belong to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "aa29c7f1-9279-428c-bba5-8ea86e9fa3ce",
          "name": "getPropertyIdList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/id?geoid=%7B%7D&maxBeds=%7B%7D&minBeds=%7B%7D&orderby=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of property IDs within a specific geography that have a specific number of beds. Use orderby to choose how you want your results sorted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32e2b498-edec-438c-bb91-7ba5a24de87e"
            }
          ]
        },
        {
          "id": "0e9b1343-66c8-450d-b969-32fe8f2c2897",
          "name": "propertyDetails",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detail?address=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b859b28-1389-4885-81c1-643932b52aa6"
            }
          ]
        },
        {
          "id": "5b912be2-2aa1-4658-a6be-8c0c501375a1",
          "name": "adressList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/address?address1=%7B%7D&address2=%7B%7D&orderby=%7B%7D&page=%7B%7D&pagesize=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of properties within a zip code. Use propertytype and order by to narrow down your results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ed2b426-6739-40c4-aca0-24b1d93b98ba"
            }
          ]
        },
        {
          "id": "bee9fbe3-1c80-488b-99e6-358f2bc6efe1",
          "name": "propertySnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/snapshot?cityname=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&maxavmvalue=%7B%7D&maxLotSize1=%7B%7D&maxtaxamt=%7B%7D&minavmvalue=%7B%7D&minLotSize1=%7B%7D&mintaxamt=%7B%7D&orderby=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of property snapshots within a specific city that are within a desired size range and a specific property type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "232b223b-9374-4a00-8330-c2e6113b01a5"
            }
          ]
        },
        {
          "id": "c7b198ed-bc24-4f36-97a1-6a38f9a3367d",
          "name": "propertyBasicProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/basicprofile?attomid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get basic property information and most recent transaction and taxes for a specific attom id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f45b754-4ad5-4b4b-8487-22f2b8e16a33"
            }
          ]
        },
        {
          "id": "8551a28c-52b0-406a-bcb4-9bb1dae2c936",
          "name": "propertyExpandedProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/expandedprofile?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a detailed property information and most recent transaction and taxes for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c54093bf-0a07-4174-8d8b-6e7c01a4dd1c"
            }
          ]
        },
        {
          "id": "99063e3c-a025-4dcd-b0ca-52feb6e5011a",
          "name": "getAllEventsDetailAddress",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/allevents/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "API Security Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a detail of all the events on a specific property based on its address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7dc9ecd3-3e0e-40b6-8e44-024c624173a2"
            }
          ]
        },
        {
          "id": "a383398a-69a2-46e0-a0b3-1eb13278ad6e",
          "name": "propertyDetailsMortage",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailmortgage?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details mortgage based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17b2b3a1-f1d2-4f0a-b992-afe72b5d56d4"
            }
          ]
        },
        {
          "id": "18c743ce-be0f-4eaa-8156-c8e599a58ad3",
          "name": "propertyDetailsOwner",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailowner?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details owner based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04c13c48-d5eb-4c78-8f28-2a5f9a9507c3"
            }
          ]
        },
        {
          "id": "362b2aa0-68e7-486b-84a7-6ed2663dc525",
          "name": "propertyDetailsMortgageOwner",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailmortgageowner?address1=%7B%7D&address2=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get property details mortgageowner based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bfb47ef-8bc2-4ba3-8f2c-33e3e2f85c5d"
            }
          ]
        },
        {
          "id": "2c23caeb-00f6-484b-b953-6d7f214a93a1",
          "name": "getAssessmentSnapshotTotal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessment/snapshot?address1=%7B%7D&address2=%7B%7D&maxmktttlvalue=%7B%7D&minmktttlvalue=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get snapshots of the properties within a radius of a property that have a total market value within a specified range."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c152abc-e613-4825-90b0-164c5931bf5d"
            }
          ]
        },
        {
          "id": "8ed2e348-0a6a-421c-8f30-ed96c2ccd324",
          "name": "assessmenDetailPropertyId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessment/detail?postalcode=%7B%7D&propertytype=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get assessment details for properties within a zip code. Use propertytpe to select a specific property type for your search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3061a5e0-f8cf-46b1-b003-cd3870a92cb8"
            }
          ]
        },
        {
          "id": "517ba361-484e-4b43-8434-fe341c880e34",
          "name": "assessmentHistoryDetailID",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/assessmenthistory/detail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a full detail of property characteristics and assessment history information for a specific property."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b07327a-d719-4d44-bab1-91417bd26f2e"
            }
          ]
        },
        {
          "id": "b3df4799-d254-492c-90bc-f1d01ce0b596",
          "name": "avmSnapshotGeoID",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/avm/snapshot?geoid=%7B%7D&maxavmvalue=%7B%7D&minavmvalue=%7B%7D&propertytype=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of AVM snapshot records that fall within an Onboard GeoID with a specific value range. Use propertytpe to select a specific property type for your search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8345cac-01af-467e-b4a3-ca2fc142a5bc"
            }
          ]
        },
        {
          "id": "5a51c33d-2349-4948-a831-1beea411582c",
          "name": "avmDetailPostal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/avm/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get AVM details for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f74cd73-4d7c-4831-9fc4-7aa4838af214"
            }
          ]
        },
        {
          "id": "9aec7aac-f555-4425-978a-2682fe680657",
          "name": "attomAvmDetail",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/attomavm/detail?attomid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Attomized AVM and other property details for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7022008-5c32-4f8e-a5ad-0b7ccf73c239"
            }
          ]
        },
        {
          "id": "c89fb1e2-dd70-4843-a7db-4487a6b04359",
          "name": "getHomeSaleSnapshotsGeoId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/sale/snapshot?address1=%7B%7D&address2=%7B%7D&endsalesearchdate=%7B%7D&geoid=%7B%7D&maxsaleamt=%7B%7D&minsaleamt=%7B%7D&propertytype=%7B%7D&radius=%7B%7D&startsalesearchdate=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of home sale snapshots within a Onboard GeoID that sold within a date range and specified sale amount."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "258dea58-ac8c-4597-a1fc-3c39fe8ca12c"
            }
          ]
        },
        {
          "id": "99ba1a2c-8e25-4358-9a33-f8e72d007714",
          "name": "getSaleDetailPostal",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/sale/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get sales information for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb8837a8-bea6-411a-b047-69f97e5fe627"
            }
          ]
        },
        {
          "id": "89deed89-ad56-445f-8fb4-c184752f0d12",
          "name": "getSaleHistorySnapshotPropertyId",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/snapshot?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a sales history snapshot of a property based on an Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca134d15-a3cc-4e88-9f05-e7130ed25ac9"
            }
          ]
        },
        {
          "id": "b665c5a7-2bac-406a-9ec9-bdede37c527d",
          "name": "saleHistoryBasicHistory",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/basichistory?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the basic transaction and loan history on a property for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6526d5a1-1495-4a34-bd31-7a2110be8d88"
            }
          ]
        },
        {
          "id": "01d04bba-40ce-4f4b-abd2-4962174ad66c",
          "name": "saleHistoryExpandedHistory",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/expandedhistory?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the detailed transaction, pre-foreclosure and loan history on a property for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57e9cc46-6658-4ad2-8534-ffba74f50bee"
            }
          ]
        },
        {
          "id": "0f6522b7-dc0c-43b6-8f57-b7b2d259775a",
          "name": "getSaleHistoryDetailAddress",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/saleshistory/detail?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a sales history snapshot of a property based on an address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac4fa0ac-2256-4826-903a-19e21f3503b7"
            }
          ]
        },
        {
          "id": "476e71c7-9853-4271-80dd-9200ac4ac3d5",
          "name": "getSalesTrendByYear",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/salestrend/snapshot?endmonth=%7B%7D&endyear=%7B%7D&geoid=%7B%7D&interval=%7B%7D&startmonth=%7B%7D&startyear=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the average sale price, median sale price, and count of sales for the past 2 years in yearly intervals."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c46c5868-9e57-4b68-ba11-b8cb9d163e3d"
            }
          ]
        },
        {
          "id": "e37d5c91-715c-419a-9bff-3d799f1ee498",
          "name": "getAreaHierarchyLookup",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/hierarchy/lookup?geoType=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&WKTString=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This method allows you to pass a latitude and longitude point and geo type to retrieve a list of geographies that point falls within. Required input is a valid WKT (Well Known Text) point."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0f34cf4-717d-4713-ac0b-98dc30a16f42"
            }
          ]
        },
        {
          "id": "e5d9033a-1477-4cfb-aa9b-0240cc381e99",
          "name": "getPOISearchGeography",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/poi/geography?PostalCodeKey=%7B%7D&RecordLimit=%7B%7D&SearchDistance=%7B%7D&Sort=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This search returns a list of Points of Interest in proximity to the centroid of a zip code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fc5f81e-a42e-4da8-809f-ea8754227e23"
            }
          ]
        },
        {
          "id": "58661657-6626-4da6-8334-e3482edebeb6",
          "name": "getPOISearchPoint",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/poi/point?BusinessCategory=%7B%7D&Point=%7B%7D&RecordLimit=%7B%7D&SearchDistance=%7B%7D&Sort=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This search returns a list of POI in proximity to a latitude/longitude."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6313dd0-edb7-4b1c-9264-88117fcbfe0b"
            }
          ]
        },
        {
          "id": "00e9c4d3-0020-45fd-bcf4-93afd85dbb5e",
          "name": "getPOISearchPoint",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/poi/street+address?RecordLimit=%7B%7D&SearchDistance=%7B%7D&Sort=%7B%7D&StreetAddress=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This search returns a list of POI in proximity to an address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8457d793-7bdf-444e-9a4a-c65130367561"
            }
          ]
        },
        {
          "id": "5d382492-e8f4-4c33-806d-417badeca824",
          "name": "getPOIBusinessCategoryLookup",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/business+category/lookup",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This lookup is used to obtain a full list of Business Categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3c1c309-c74f-45c9-a610-996bb1c013e1"
            }
          ]
        },
        {
          "id": "5de4d251-a526-499a-b434-d6f26e53a645",
          "name": "getPOIlob",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/lob/lookup",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This lookup can be used to show the full list of Lines of Businesses (LOB), and which categories they belong to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8a05a8d-2665-4edc-ba85-dc1079aad054"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "9b1b338e-c0a7-4ead-bf9f-a0cf34a72048",
          "name": "propertyDetailsWithSchools",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailwithschools?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search for a property to have the property details returned, along with the schools in the associated attendance zones."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "828cd58b-b4ef-449f-8864-450f4fa31c3c"
            }
          ]
        },
        {
          "id": "ad617803-c0c9-46cf-a69e-b307ab3a05d6",
          "name": "propertySchoolSnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/snapshot?filetypetext=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search for all schools that are located within a given radius around a given latitude and longitude."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c2e0590-7563-4d80-8a3c-9058ea7e2f8e"
            }
          ]
        },
        {
          "id": "3a77cdb0-c471-46fd-a362-746cff53f7a3",
          "name": "propertyDetails",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/detail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search by school ID to return all of the available details about a school"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d217ddd-c3b3-44f8-9c3e-0a1c5a1fea3d"
            }
          ]
        },
        {
          "id": "0d4bd5fb-b9ea-4474-a43f-17418caeae1c",
          "name": "propertySchoolDistrictDetail",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/districtdetail?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search by district number to return all of the available details about a school district"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c7b30ea-fbb5-492f-9cac-1e625a87955f"
            }
          ]
        }
      ]
    }
  ]
}