{
  "info": {
    "name": "Amazon DynamoDB API Describe Limits",
    "_postman_id": "55bd6674-f4b3-42ec-9977-a865774baa77",
    "description": "Returns the current provisioned-capacity limits for your AWS account in a region, both for the region as a whole and for any one DynamoDB table that you create there.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "73188a86-e977-4166-902b-a78233ef7ea7",
          "name": "batchGetItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchGetItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchGetItem operation returns the attributes of one or more items from one or\n      more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a63acb9-fe47-4372-8021-92b799661f23"
            }
          ]
        },
        {
          "id": "909d7d37-9539-4d70-b370-0c10c035bd20",
          "name": "batchWriteItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchWriteItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchWriteItem operation puts or deletes multiple items in one or more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98f8dc96-1946-4f41-8d36-be163b16ced0"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "afa0444d-0e80-4c78-af6f-580699e06e77",
          "name": "createTable",
          "request": {
            "url": "http://example.com/api/?Action=CreateTable?AttributeDefinitions=AttributeDefinitions&GlobalSecondaryIndexes=GlobalSecondaryIndexes&KeySchema=KeySchema&LocalSecondaryIndexes=LocalSecondaryIndexes&ProvisionedThroughput=ProvisionedThroughput&StreamSpecification=StreamSpecification&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The CreateTable operation adds a new table to your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1b38b12-38a5-40a5-b7b1-0c052aa80cf2"
            }
          ]
        },
        {
          "id": "554e0105-60ec-4aae-860e-4a25c17c0c6d",
          "name": "deleteTable",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTable?TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteTable operation deletes a table and all of its items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc4b31db-edcb-44b7-9fa3-6d8a43d48e7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "ff57d03a-aab9-48dc-82c0-ffe5300d2342",
          "name": "deleteItem",
          "request": {
            "url": "http://example.com/api/?Action=DeleteItem?ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Key=Key&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a single item in a table by primary key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f35d1fb-d65a-4cdd-8950-730e2a0ef753"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "6d0c61c5-9322-4409-95af-49c2f67cc404",
          "name": "describeLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLimits?AccountMaxReadCapacityUnits=AccountMaxReadCapacityUnits&AccountMaxWriteCapacityUnits=AccountMaxWriteCapacityUnits&TableMaxReadCapacityUnits=TableMaxReadCapacityUnits&TableMaxWriteCapacityUnits=TableMaxWriteCapacityUnits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current provisioned-capacity limits for your AWS account in a region, both for the region as a whole and for any one DynamoDB table that you create there."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36bdc0df-5443-4044-bf25-faecedfa290c"
            }
          ]
        }
      ]
    }
  ]
}