{
  "info": {
    "name": "AWS Cognito API Describe User Pool",
    "_postman_id": "13c11355-3a6e-4ce6-b4ac-fbe8ea182e32",
    "description": "Returns the configuration information and metadata of the specified user\n            pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "068287c7-a562-4ef4-9eee-0c1081a02086",
          "name": "createUserPool",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPool?AdminCreateUserConfig=AdminCreateUserConfig&AliasAttributes=AliasAttributes&AutoVerifiedAttributes=AutoVerifiedAttributes&DeviceConfiguration=DeviceConfiguration&EmailConfiguration=EmailConfiguration&EmailVerificationMessage=EmailVerificationMessage&EmailVerificationSubject=EmailVerificationSubject&LambdaConfig=LambdaConfig&MfaConfiguration=MfaConfiguration&Policies=Policies&PoolName=PoolName&Schema=Schema&SmsAuthenticationMessage=SmsAuthenticationMessage&SmsConfiguration=SmsConfiguration&SmsVerificationMessage=SmsVerificationMessage&UserPoolTags=UserPoolTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Cognito user pool and sets the password policy for the\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8635004-d135-44c0-a02c-503454ddc026"
            }
          ]
        },
        {
          "id": "70c6d205-c347-4482-b234-1dca641e7903",
          "name": "deleteUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Amazon Cognito user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9830edac-d2e1-40e0-ac83-996a0114993c"
            }
          ]
        },
        {
          "id": "f81553c8-cb87-42af-9823-c083c5d2809b",
          "name": "deleteUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the developer to delete the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a92a2d3-0088-4f09-9a9c-512cb399a59b"
            }
          ]
        },
        {
          "id": "9b27e9c1-7c81-4c9f-9e98-2ede5b1373de",
          "name": "describeUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the configuration information and metadata of the specified user\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16f9904c-7bfb-42b5-8fc4-45fb3adf20d4"
            }
          ]
        }
      ]
    }
  ]
}