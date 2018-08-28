{
  "info": {
    "name": "AWS Kinesis Analytics API List Applications",
    "_postman_id": "5918170b-a672-4f12-815b-317af3aa0605",
    "description": "Returns a list of Amazon Kinesis Analytics applications in your account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "9fb20759-f24b-4c01-9e7e-731e9b329b77",
          "name": "addApplicationInput",
          "request": {
            "url": "http://example.com/api/?Action=AddApplicationInput?ApplicationName=ApplicationName&CurrentApplicationVersionId=CurrentApplicationVersionId&Input=Input",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a streaming source to your Amazon Kinesis application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43c0b5e9-5028-4d9a-a343-3b603c97fd5e"
            }
          ]
        },
        {
          "id": "6ae9fc02-7f38-4010-b5e7-8218744067e1",
          "name": "addApplicationOutput",
          "request": {
            "url": "http://example.com/api/?Action=AddApplicationOutput?ApplicationName=ApplicationName&CurrentApplicationVersionId=CurrentApplicationVersionId&Output=Output",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an external destination to your Amazon Kinesis Analytics application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebc29c78-6aaf-4b3c-810a-0c533a549d29"
            }
          ]
        },
        {
          "id": "d71ece63-110c-4e2f-8e56-71bfde1fd483",
          "name": "addApplicationReferenceDataSource",
          "request": {
            "url": "http://example.com/api/?Action=AddApplicationReferenceDataSource?ApplicationName=ApplicationName&CurrentApplicationVersionId=CurrentApplicationVersionId&ReferenceDataSource=ReferenceDataSource",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a reference data source to an existing application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0720934-10c4-4823-953b-e44f6651917e"
            }
          ]
        },
        {
          "id": "fb7ed524-22a8-4abf-8fea-456592d3a340",
          "name": "createApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreateApplication?ApplicationCode=ApplicationCode&ApplicationDescription=ApplicationDescription&ApplicationName=ApplicationName&Inputs=Inputs&Outputs=Outputs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Amazon Kinesis Analytics application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02eb29a9-224e-4e19-9a5e-efc100ace6b7"
            }
          ]
        },
        {
          "id": "f18e462c-4b58-41fc-9f4e-6682c678b454",
          "name": "deleteApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApplication?ApplicationName=ApplicationName&CreateTimestamp=CreateTimestamp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7004ef4e-50f0-4b76-99c6-99885ad12fdd"
            }
          ]
        },
        {
          "id": "89bd4e0e-bdbc-4556-9369-dbfef85530ea",
          "name": "deleteApplicationOutput",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApplicationOutput?ApplicationName=ApplicationName&CurrentApplicationVersionId=CurrentApplicationVersionId&OutputId=OutputId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes output destination configuration from your application configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9db17147-3579-4aab-aa2c-27bc4d582ebf"
            }
          ]
        },
        {
          "id": "4e5fd357-763f-49a0-b9a8-b7fb9f078f45",
          "name": "deleteApplicationReferenceDataSource",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApplicationReferenceDataSource?ApplicationName=ApplicationName&CurrentApplicationVersionId=CurrentApplicationVersionId&ReferenceId=ReferenceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a reference data source configuration from the specified application configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e04d3a0-5b41-4889-b6c8-53eaf60818e0"
            }
          ]
        },
        {
          "id": "f89a1106-db1c-42ea-9e4d-d4bdd95bc2d8",
          "name": "describeApplication",
          "request": {
            "url": "http://example.com/api/?Action=DescribeApplication?ApplicationName=ApplicationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific Amazon Kinesis Analytics application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66755ee3-3e23-4309-9d5d-82377a67caa9"
            }
          ]
        },
        {
          "id": "fc70fba1-c765-4fb6-a2be-4de9f47a3071",
          "name": "listApplications",
          "request": {
            "url": "http://example.com/api/?Action=ListApplications",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Amazon Kinesis Analytics applications in your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26696a4a-d936-4f88-9743-ad02962cc066"
            }
          ]
        }
      ]
    }
  ]
}