{
  "info": {
    "name": "AWS Simple Notification Service API List Subscriptions",
    "_postman_id": "55c6e8ab-f692-4188-9577-4a3a4d18cdfa",
    "description": "Returns a list of the requester's subscriptions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "aac1f201-d277-486d-9012-a4a0dace834f",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?ActionName.member.N=ActionName.member.N&AWSAccountId.member.N=AWSAccountId.member.N&Label=Label&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a statement to a topic's access control policy, granting access for the specified AWS accounts to the specified actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "081b6fa4-969e-4b19-b350-98d904f522aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "9fc5c97b-cb39-41c0-afe0-7546373b0f34",
          "name": "checkIfPhoneNumberIsOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=CheckIfPhoneNumberIsOptedOut?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a phone number and indicates whether the phone holder has opted out of receiving SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95e3502e-a0e7-4a31-94a6-f8576e4c6ec6"
            }
          ]
        },
        {
          "id": "8d8a5798-af7a-44dd-9bff-de0d8ba953e7",
          "name": "listPhoneNumbersOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=ListPhoneNumbersOptedOut?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of phone numbers that are opted out, meaning you cannot send SMS messages to them."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26257f53-fa8d-4ffd-9d28-0ab6201c1f0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "42b7533e-e8c5-472f-987a-228f63894a98",
          "name": "confirmSubscription",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSubscription?AuthenticateOnUnsubscribe=AuthenticateOnUnsubscribe&Token=Token&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies an endpoint owner's intent to receive messages by validating the token sent to the\n      endpoint by an earlier Subscribe action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd2db993-b94c-4ea0-be47-29c6621feb7d"
            }
          ]
        },
        {
          "id": "41e40b7c-f4e2-4602-9093-23b5ec896c38",
          "name": "getSubscriptionAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSubscriptionAttributes?SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8d11fd8-6012-455c-9f0d-bf536cdfc39a"
            }
          ]
        },
        {
          "id": "30e2c401-42bd-43eb-a02b-c75629199f39",
          "name": "listSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptions?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65f054d4-e22b-4827-9cf2-4f4f1b11609b"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Applications",
      "item": [
        {
          "id": "0cbd7b2f-c56a-42f1-8222-6f2ce0e42218",
          "name": "createPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformApplication?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&Name=Name&Platform=Platform",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a platform application object for one of the supported push notification services,\n      such as APNS and GCM, to which devices and mobile apps may register."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c812271-2494-4e15-846a-cbc61fafc705"
            }
          ]
        },
        {
          "id": "ea6b4dc9-abe4-4e65-8c83-3bbc036589fe",
          "name": "deletePlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeletePlatformApplication?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a platform application object for one of the supported push notification services,\n      such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27dfb56d-ba37-41b4-9b00-16f789a77002"
            }
          ]
        },
        {
          "id": "4783f53a-1343-48f0-b63f-65e644001f0c",
          "name": "getPlatformApplicationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetPlatformApplicationAttributes?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the attributes of the platform application object for the supported push\n      notification services, such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d7af4a8-060c-4d85-bc52-ac9809f6ce0f"
            }
          ]
        },
        {
          "id": "01ef2af3-c86e-4bc6-bde6-2482b2fea19c",
          "name": "listPlatformApplications",
          "request": {
            "url": "http://example.com/api/?Action=ListPlatformApplications?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the platform application objects for the supported push notification services, such as\n      APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6883b30-ac7f-4b2d-8c75-fcef11fa44fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Endpoints",
      "item": [
        {
          "id": "15beb054-ad0b-481a-902d-65285db2285d",
          "name": "createPlatformEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformEndpoint?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&CustomUserData=CustomUserData&PlatformApplicationArn=PlatformApplicationArn&Token=Token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an endpoint for a device and mobile app on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f590dfdb-47aa-4ea4-a533-2a8fb2fe9788"
            }
          ]
        }
      ]
    },
    {
      "name": "Topics",
      "item": [
        {
          "id": "aa926f53-d0e6-49fd-9f87-425226dd6843",
          "name": "createTopic",
          "request": {
            "url": "http://example.com/api/?Action=CreateTopic?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a topic to which notifications can be published."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6db0c709-7e08-4b9e-be77-9b0993400b3f"
            }
          ]
        },
        {
          "id": "20dfd6da-9a6f-4874-9e41-c9a0702048d0",
          "name": "deleteTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTopic?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a topic and all its subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ef9c0ea-483b-4b6f-8c8e-161727def0e0"
            }
          ]
        },
        {
          "id": "bb92d79b-20fb-48d9-97ee-3efcee703266",
          "name": "getTopicAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetTopicAttributes?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf405bf9-fab6-45d9-8145-582ae16dde6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "26294152-8940-4336-83a8-4778a877dea5",
          "name": "deleteEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEndpoint?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the endpoint for a device and mobile app from Amazon SNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "102da0ac-8ec7-4840-b8dc-82b80e24dc84"
            }
          ]
        },
        {
          "id": "a99b6653-e55a-4ae8-bdfd-0ac88d86a442",
          "name": "getEndpointAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetEndpointAttributes?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the endpoint attributes for a device on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6d4c1cb-f504-440e-8910-e1e85a7af195"
            }
          ]
        },
        {
          "id": "41a7b42c-ebb1-43d8-a4fd-4ff0b513e97f",
          "name": "listEndpointsByPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=ListEndpointsByPlatformApplication?NextToken=NextToken&PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the endpoints and endpoint attributes for devices in a supported push notification\n      service, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "381dd5bf-da78-403c-8b4c-317172f42377"
            }
          ]
        }
      ]
    },
    {
      "name": "SMS",
      "item": [
        {
          "id": "3509e3b3-90a0-48bd-b419-c0df33b839cb",
          "name": "getSMSAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSMSAttributes?attributes.member.N=attributes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the settings for sending SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6b20ae9-ea80-4040-bbac-37e148df2297"
            }
          ]
        }
      ]
    }
  ]
}