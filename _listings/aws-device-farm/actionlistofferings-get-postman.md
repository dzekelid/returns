{
  "info": {
    "name": "AWS Device Farm API List Offerings",
    "_postman_id": "6d47edd0-acda-434c-918d-09c4a603895b",
    "description": "Returns a list of products or offerings that the user can manage through the API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "19732a2d-e6e0-4158-94a0-edab357269a3",
          "name": "createDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=CreateDevicePool?description=description&name=name&projectArn=projectArn&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3baa67c7-0e05-47ba-a63c-8ce2ae0cb7ba"
            }
          ]
        },
        {
          "id": "d4dff62c-42d1-4f79-92f8-df691ad2d2dc",
          "name": "deleteDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device pool given the pool ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "505516fd-698c-473d-8366-696e1ba2d299"
            }
          ]
        },
        {
          "id": "1b029444-846c-4a21-b3a0-2ec81194261f",
          "name": "getDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b4c6fbe-d2bb-4403-afbe-5b3c9fe4e2d6"
            }
          ]
        },
        {
          "id": "a794c7df-a5af-4213-8635-bb64556b275a",
          "name": "getDevicePoolCompatibility",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePoolCompatibility?appArn=appArn&devicePoolArn=devicePoolArn&testType=testType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about compatibility with a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83bb6768-0a00-49cb-b32a-67fd5fb3b7b8"
            }
          ]
        },
        {
          "id": "0542a74e-3ab2-4f93-ab10-cd9e3f45ad69",
          "name": "listDevicePools",
          "request": {
            "url": "http://example.com/api/?Action=ListDevicePools?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about device pools."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "702c576c-8e3b-43be-8260-04d2ab90d21f"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "70ae7858-bfba-4ebb-baa1-11b0d59ac51b",
          "name": "createProject",
          "request": {
            "url": "http://example.com/api/?Action=CreateProject?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "005b60ce-828e-46ac-953f-2db218bf95b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "c3e387a4-dd7c-400b-9508-369006b63186",
          "name": "createRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=CreateRemoteAccessSession?configuration=configuration&deviceArn=deviceArn&name=name&projectArn=projectArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies and starts a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5df5a871-38ac-4e25-949f-d0ae5c6a0fe5"
            }
          ]
        },
        {
          "id": "f0c2e813-efb5-46d7-a65c-34257d0a13c4",
          "name": "deleteRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a completed remote access session and its results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12b0ca54-44e4-49c0-aec4-0e8af3f3e382"
            }
          ]
        },
        {
          "id": "9767fffe-94c4-4204-8956-30272f1cb377",
          "name": "getRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=GetRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a link to a currently running remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8eaf7eef-fad2-4fb9-b6ae-ee108c86abb0"
            }
          ]
        },
        {
          "id": "1b215b89-3b4c-4678-8750-b173a8766963",
          "name": "installToRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=InstallToRemoteAccessSession?appArn=appArn&remoteAccessSessionArn=remoteAccessSessionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an application to the device in a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a4f33a0-9770-41f2-8573-c4e3a7ea9f28"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "af261991-1778-45e4-9c5d-1f8db3e86b2a",
          "name": "createUpload",
          "request": {
            "url": "http://example.com/api/?Action=CreateUpload?contentType=contentType&name=name&projectArn=projectArn&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads an app or test scripts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "531ab240-2d5c-4ba1-bcf3-3dbcf4828639"
            }
          ]
        },
        {
          "id": "d556d04c-7d3e-4e0f-b15a-4bef3ba55bf7",
          "name": "getUpload",
          "request": {
            "url": "http://example.com/api/?Action=GetUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about an upload."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99d71794-afa6-4f64-83e1-163e55e8d474"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "b2e8181a-8d67-47ab-b5f3-69557d1520b8",
          "name": "deleteProject",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Device Farm project, given the project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54ffa5b9-af9b-4065-a17f-447588f6f855"
            }
          ]
        },
        {
          "id": "c003dafe-cf86-4524-9eff-36121a141747",
          "name": "getProject",
          "request": {
            "url": "http://example.com/api/?Action=GetProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9ef3555-6ddd-421c-968c-b716b2881811"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "fbc81b1f-e048-4183-a08e-f02a9c20b3fd",
          "name": "deleteRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the run, given the run ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34816de7-a8f1-4ec4-b1b2-9652e6b09b3b"
            }
          ]
        },
        {
          "id": "56705f22-2446-4009-beb9-629b187ecad5",
          "name": "getRun",
          "request": {
            "url": "http://example.com/api/?Action=GetRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f10fdf8f-3d23-4c84-b36a-d26f1ef656d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "90b28829-a67a-40c9-a256-2089f6058375",
          "name": "deleteUpload",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an upload given the upload ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5de997da-1918-4008-a97e-3ac7df3675ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "9ed86702-946e-4c2b-838b-b9246a167a01",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?accountSettings=accountSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of unmetered iOS and/or unmetered Android devices that have been purchased by the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d77a383b-0dea-4ada-b506-ae983836d863"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "e98bea6f-a2f6-4ef0-8a6f-b947e3a2bd51",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a unique device type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28252850-3796-4989-a482-b7650e085910"
            }
          ]
        },
        {
          "id": "fa707f3e-9fbb-4646-b99c-1b4931d2fb71",
          "name": "listDevices",
          "request": {
            "url": "http://example.com/api/?Action=ListDevices?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about unique device types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d91f872-f6a0-46d9-af9a-7e06fac8ca4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "ee116d3f-bb4c-4e22-bfb9-3002b2aa8158",
          "name": "getJob",
          "request": {
            "url": "http://example.com/api/?Action=GetJob?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ade7b1c-5a98-40ee-a903-2ee556ed2436"
            }
          ]
        },
        {
          "id": "17cae928-048d-49d6-96b6-f4af611fb8ca",
          "name": "listJobs",
          "request": {
            "url": "http://example.com/api/?Action=ListJobs?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fa707ee-2691-4c4d-8217-9b9d3c0853a5"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "eba7f840-1d15-4b4b-87fe-4fab6eb48faa",
          "name": "getOfferingStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetOfferingStatus?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the current status and future status of all offerings purchased by an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ced81f6-3ed4-4d1c-a060-c4489be1c129"
            }
          ]
        }
      ]
    },
    {
      "name": "Suites",
      "item": [
        {
          "id": "b53a0c96-70ce-4101-b4fd-ee100b8a3743",
          "name": "getSuite",
          "request": {
            "url": "http://example.com/api/?Action=GetSuite?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a suite."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba89532c-0122-4f7e-9abb-d963946a0416"
            }
          ]
        }
      ]
    },
    {
      "name": "Tests",
      "item": [
        {
          "id": "5235ec7b-8373-4b8e-9b49-ace6a0e9c2e0",
          "name": "getTest",
          "request": {
            "url": "http://example.com/api/?Action=GetTest?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a test."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff66be6b-a804-4200-b562-9ae152a000cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Artifacts",
      "item": [
        {
          "id": "c23eb502-ba4c-4293-ac9d-c1c2366c0ba7",
          "name": "listArtifacts",
          "request": {
            "url": "http://example.com/api/?Action=ListArtifacts?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about artifacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50e6f6ff-89fa-46fa-9ac3-12e61627ac28"
            }
          ]
        }
      ]
    },
    {
      "name": "Offerings",
      "item": [
        {
          "id": "801eac4b-3b0d-455a-96c3-af766988bd4c",
          "name": "listOfferings",
          "request": {
            "url": "http://example.com/api/?Action=ListOfferings?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of products or offerings that the user can manage through the API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac34bf54-759c-41d5-a5c6-4b3f38f6967c"
            }
          ]
        }
      ]
    }
  ]
}