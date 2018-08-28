{
  "info": {
    "name": "AWS Snowball API Get Snowball Usage",
    "_postman_id": "c66ec0dd-37a3-4dbb-a737-2752997291eb",
    "description": "Returns information about the Snowball service limit for your account, and also the\n      number of Snowballs your account has in use.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "1639fb31-33b9-4900-9c3f-a9b23e61525b",
          "name": "cancelCluster",
          "request": {
            "url": "http://example.com/api/?Action=CancelCluster?ClusterId=ClusterId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a cluster job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28b12f3c-eb4a-481f-9fdd-1355383eec86"
            }
          ]
        },
        {
          "id": "aa8e862f-6d2a-4265-a89c-3fe100fd8b1d",
          "name": "createCluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateCluster?AddressId=AddressId&Description=Description&JobType=JobType&KmsKeyARN=KmsKeyARN&Notification=Notification&Resources=Resources&RoleARN=RoleARN&ShippingOption=ShippingOption&SnowballType=SnowballType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9acbe8b0-d253-4c25-9843-cd0614d76b72"
            }
          ]
        },
        {
          "id": "b40e99cb-4c28-4f0b-931b-3bf844169a3c",
          "name": "describeCluster",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCluster?ClusterId=ClusterId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific cluster including shipping information, cluster\n      status, and other important metadata."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54d95502-534a-4162-a92d-1aa6b17ae05d"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "e8c17396-d0ed-4186-b4af-c2aeeceecf6c",
          "name": "cancelJob",
          "request": {
            "url": "http://example.com/api/?Action=CancelJob?JobId=JobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels the specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c80e9efe-d5f4-4469-9685-01c0e24ca923"
            }
          ]
        },
        {
          "id": "6fce17c3-a247-461b-8fa6-e9cac044dca0",
          "name": "createJob",
          "request": {
            "url": "http://example.com/api/?Action=CreateJob?AddressId=AddressId&ClusterId=ClusterId&Description=Description&JobType=JobType&KmsKeyARN=KmsKeyARN&Notification=Notification&Resources=Resources&RoleARN=RoleARN&ShippingOption=ShippingOption&SnowballCapacityPreference=SnowballCapacityPreference&SnowballType=SnowballType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a job to import or export data between Amazon S3 and your on-premises data\n      center."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e1bbdb8-6e00-40b4-b834-3680164ecb6d"
            }
          ]
        },
        {
          "id": "2ab96209-c4c7-47c3-bc3e-8fcf8faf73e9",
          "name": "describeJob",
          "request": {
            "url": "http://example.com/api/?Action=DescribeJob?JobId=JobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific job including shipping information, job status,\n      and other important metadata."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c1c8698-da14-4949-935e-9dea76fdccb5"
            }
          ]
        },
        {
          "id": "821297f7-ba67-4c64-8a99-1895e13a7a10",
          "name": "getJobUnlockCode",
          "request": {
            "url": "http://example.com/api/?Action=GetJobUnlockCode?JobId=JobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the UnlockCode code value for the specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c24b668b-b4d2-4a2b-b9be-1b2f10a2f125"
            }
          ]
        }
      ]
    },
    {
      "name": "Addresses",
      "item": [
        {
          "id": "ecea2209-10e4-4af9-803e-163661a259ca",
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
              "id": "344e6809-f59c-47b0-b671-413e3e20396c"
            }
          ]
        },
        {
          "id": "0b0a820d-027c-4e44-bb3c-e3da9c0bd19c",
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
              "id": "29eb6420-c437-4f1a-b2dd-caf77c21db3b"
            }
          ]
        },
        {
          "id": "c35b32bd-d327-4605-a179-79bbdc1b047c",
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
              "id": "7a4de166-abae-464c-a362-ac23d66705e7"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Manifest",
      "item": [
        {
          "id": "456e62bd-d5cb-4141-85fa-31dcb843397b",
          "name": "getJobManifest",
          "request": {
            "url": "http://example.com/api/?Action=GetJobManifest?JobId=JobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a link to an Amazon S3 presigned URL for the manifest file associated with the\n      specified JobId value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36489ad7-230a-4615-bd45-8e6eaf99340a"
            }
          ]
        }
      ]
    },
    {
      "name": "Usage",
      "item": [
        {
          "id": "d266d01c-3d4f-4057-92e0-b6bba9995783",
          "name": "getSnowballUsage",
          "request": {
            "url": "http://example.com/api/?Action=GetSnowballUsage?SnowballLimit=SnowballLimit&SnowballsInUse=SnowballsInUse",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the Snowball service limit for your account, and also the\n      number of Snowballs your account has in use."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e638176-0952-44fa-922c-4a9809765a81"
            }
          ]
        }
      ]
    }
  ]
}