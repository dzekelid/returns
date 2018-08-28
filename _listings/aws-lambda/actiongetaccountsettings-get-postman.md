{
  "info": {
    "name": "AWS Lambda API Get Account Settings",
    "_postman_id": "a1e02ef6-b306-49a1-8c49-77dd0b071954",
    "description": "Returns a customer's account settings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "ee1d0cc1-8fd1-4e45-bd05-57226a90444b",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?FunctionName=FunctionName&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a permission to the resource policy associated with the specified AWS Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "984720a7-18bf-4f23-b736-1d12d7d5671f"
            }
          ]
        }
      ]
    },
    {
      "name": "Aliases",
      "item": [
        {
          "id": "ab24dd74-7fde-437a-8e84-a152aea4b14b",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?FunctionName=FunctionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias that points to the specified Lambda function version."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0b2fd36-a05a-48c6-bba9-2171029195d2"
            }
          ]
        },
        {
          "id": "e9d38b61-de93-48b8-9e04-e12aee978014",
          "name": "deleteAlias",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAlias?FunctionName=FunctionName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Lambda function alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5135b7f3-3114-4764-92e1-2d37dc8d46b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Sources",
      "item": [
        {
          "id": "595f13f0-55da-4090-aac2-492343e2f38f",
          "name": "createEventSourceMapping",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSourceMapping?BatchSize=BatchSize&Enabled=Enabled&EventSourceArn=EventSourceArn&FunctionName=FunctionName&StartingPosition=StartingPosition&StartingPositionTimestamp=StartingPositionTimestamp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Identifies a stream as an event source for a Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23736799-5ee6-4e10-9fe9-fccc69b8f867"
            }
          ]
        },
        {
          "id": "e8e0b780-66f7-4a03-9c95-eb14299a9daa",
          "name": "deleteEventSourceMapping",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSourceMapping?UUID=UUID",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an event source mapping."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f0879ab-4a36-42f0-b6e1-3a4671c007e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Functions",
      "item": [
        {
          "id": "dcba2dc1-f928-40d6-ab53-1fe6ebf2cd66",
          "name": "createFunction",
          "request": {
            "url": "http://example.com/api/?Action=CreateFunction?Code=Code&DeadLetterConfig=DeadLetterConfig&Description=Description&Environment=Environment&FunctionName=FunctionName&Handler=Handler&KMSKeyArn=KMSKeyArn&MemorySize=MemorySize&Publish=Publish&Role=Role&Runtime=Runtime&Timeout=Timeout&VpcConfig=VpcConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Lambda function."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb22ff54-c027-4dfa-8339-4821e5aa489b"
            }
          ]
        },
        {
          "id": "d0cca974-0627-4984-83c0-5daf0ce6dfe3",
          "name": "deleteFunction",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFunction?FunctionName=FunctionName&Qualifier=Qualifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Lambda function code and configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1598c020-a948-4b6d-a39f-1ccad5364e29"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "a95161e3-e7de-4e59-9505-f2d9e85c6a21",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?AccountLimit=AccountLimit&AccountUsage=AccountUsage",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a customer's account settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b5aeab1-a323-4bd3-aa32-5221ca3ca156"
            }
          ]
        }
      ]
    }
  ]
}