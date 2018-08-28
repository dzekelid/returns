{
  "info": {
    "name": "AWS Security Token Service API Get Caller Identity",
    "_postman_id": "4329166a-91a4-4136-9268-aeac28fbd144",
    "description": "Returns details about the IAM identity whose credentials are used to call the\n      API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Roles",
      "item": [
        {
          "id": "6df7ec36-75b2-4f5f-b1cb-4efc396c6322",
          "name": "assumeRole",
          "request": {
            "url": "http://example.com/api/?Action=AssumeRole?DurationSeconds=DurationSeconds&ExternalId=ExternalId&Policy=Policy&RoleArn=RoleArn&RoleSessionName=RoleSessionName&SerialNumber=SerialNumber&TokenCode=TokenCode",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials (consisting of an access key ID, a\n      secret access key, and a security token) that you can use to access AWS resources that you\n      might not normally have access to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4edb05ef-4578-4581-af89-e77215d35b7c"
            }
          ]
        },
        {
          "id": "4a3fa70f-4f12-4813-a1a0-a45212c60eae",
          "name": "assumeRoleWithSAML",
          "request": {
            "url": "http://example.com/api/?Action=AssumeRoleWithSAML?DurationSeconds=DurationSeconds&Policy=Policy&PrincipalArn=PrincipalArn&RoleArn=RoleArn&SAMLAssertion=SAMLAssertion",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials for users who have been authenticated\n      via a SAML authentication response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3a821d2-1fa9-4bbe-9fb9-e4cd4a43343f"
            }
          ]
        },
        {
          "id": "3483a45c-f307-40b8-bb8b-0be642293918",
          "name": "assumeRoleWithWebIdentity",
          "request": {
            "url": "http://example.com/api/?Action=AssumeRoleWithWebIdentity?DurationSeconds=DurationSeconds&Policy=Policy&ProviderId=ProviderId&RoleArn=RoleArn&RoleSessionName=RoleSessionName&WebIdentityToken=WebIdentityToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials for users who have been authenticated\n      in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,\n      Facebook, Google, or any OpenID Connect-compatible identity provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2acb3f8c-b440-47df-ad71-6ee14f3e1cd8"
            }
          ]
        },
        {
          "id": "5020e586-ffbe-4c00-a3aa-9cd93b7876cd",
          "name": "decodeAuthorizationMessage",
          "request": {
            "url": "http://example.com/api/?Action=DecodeAuthorizationMessage?EncodedMessage=EncodedMessage",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Decodes additional information about the authorization status of a request from an\n      encoded message returned in response to an AWS request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b214a420-3c25-48d6-9f12-4b3eac2b41e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "fd319115-7782-442d-b49d-7f2a7f405b10",
          "name": "getCallerIdentity",
          "request": {
            "url": "http://example.com/api/?Action=GetCallerIdentity?Account=Account&Arn=Arn&UserId=UserId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details about the IAM identity whose credentials are used to call the\n      API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea6b980d-062c-4cfc-a659-8281e9e5f904"
            }
          ]
        }
      ]
    }
  ]
}