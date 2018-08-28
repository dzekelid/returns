{
  "info": {
    "name": "AWS Security Token Service API Get Federation Token",
    "_postman_id": "882ad5eb-7343-4759-998f-087e59395774",
    "description": "Returns a set of temporary security credentials (consisting of an access key ID, a\n      secret access key, and a security token) for a federated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Roles",
      "item": [
        {
          "id": "b56f659b-3f94-4356-bd78-4d591c31672c",
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
              "id": "6740c4f6-4525-4b37-b2aa-16c042f677c3"
            }
          ]
        },
        {
          "id": "f250749b-8002-4b64-bd43-f714fafa2b55",
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
              "id": "43d074c3-ee0b-4bb1-bd98-f658fddb8598"
            }
          ]
        },
        {
          "id": "04887744-6245-468e-8779-6d763d737c88",
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
              "id": "0b668081-953b-4d0a-866d-9fffa3e7f671"
            }
          ]
        },
        {
          "id": "ab7a2b95-b6d9-4450-ada1-acf4a7fa3171",
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
              "id": "d13e238c-8816-4485-a1a5-ea0b261de6a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "77c97ca1-dd8b-4505-9b29-853cb4023a89",
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
              "id": "3404f2ea-4a89-41d1-8ca8-61f21a7f82bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Federation Token",
      "item": [
        {
          "id": "e77c15ab-6144-4040-a5dc-927b3dd4f882",
          "name": "getFederationToken",
          "request": {
            "url": "http://example.com/api/?Action=GetFederationToken?DurationSeconds=DurationSeconds&Name=Name&Policy=Policy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials (consisting of an access key ID, a\n      secret access key, and a security token) for a federated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24e9fe70-a2d0-4b63-86b2-08910c6da9bf"
            }
          ]
        }
      ]
    }
  ]
}