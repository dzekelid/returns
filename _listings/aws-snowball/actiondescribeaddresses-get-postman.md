{
  "info": {
    "name": "AWS Snowball API Describe Addresses",
    "_postman_id": "ce6b6ae3-7f12-4747-b26c-e66e03728ee0",
    "description": "Returns a specified number of ADDRESS objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Addresses",
      "item": [
        {
          "id": "51c16593-7891-46fa-abef-ffe1e279411e",
          "name": "createAddress",
          "request": {
            "url": "http://example.com/api/?Action=CreateAddress?Address=Address",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an address for a Snowball to be shipped to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f995de34-7e03-4a55-a0a7-34a83c3a03b8"
            }
          ]
        },
        {
          "id": "8aff4e71-4383-43bb-b27a-bf9be751ca6c",
          "name": "describeAddress",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAddress?AddressId=AddressId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Takes an AddressId and returns specific details about that address in the\n      form of an Address object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8cc0999-7d81-4c33-9bf4-d654de024824"
            }
          ]
        },
        {
          "id": "cde1cb82-c2b8-4b47-9a0e-8651eb421f25",
          "name": "describeAddresses",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAddresses?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a specified number of ADDRESS objects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ed6d389-aab3-4182-b872-dfeb9400fc2e"
            }
          ]
        }
      ]
    }
  ]
}