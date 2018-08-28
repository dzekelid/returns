{
  "info": {
    "name": "AWS Simple Email Service API List Identity Policies",
    "_postman_id": "0099c513-8ad5-4ea8-9ad2-8f0916c214f8",
    "description": "Returns a list of sending authorization policies that are attached to the given identity (an email address or a domain).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "cb286045-350e-43e2-b207-c8b3146cbbc0",
          "name": "cloneReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CloneReceiptRuleSet?OriginalRuleSetName=OriginalRuleSetName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule set by cloning an existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "067e924a-3f0c-4368-82d5-6893d5df35c6"
            }
          ]
        },
        {
          "id": "6ba35c70-2775-4b73-97f2-ea29eda7184d",
          "name": "createReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6b0c91f-c7f6-4b11-8836-2b95d531c528"
            }
          ]
        },
        {
          "id": "116075f8-db42-45bd-af7a-7fd006b64d07",
          "name": "deleteReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule set and all of the receipt rules it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "677d3b57-156b-4c35-b55b-99a77764cd83"
            }
          ]
        },
        {
          "id": "1b5e87f0-77bf-40df-83c3-d9cc99da057c",
          "name": "describeActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActiveReceiptRuleSet?Metadata=Metadata&Rules.member.N=Rules.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata and receipt rules for the receipt rule set that is currently active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc7e2785-5a22-405a-96a7-6d20731c9905"
            }
          ]
        },
        {
          "id": "c918618e-2a50-4075-b850-8e0868d805ad",
          "name": "describeReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e56d23d-25c0-40c1-a947-1b8ac5a70930"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "ee25568c-fc7b-4ae1-bfe9-94da82acecee",
          "name": "createConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSet?ConfigurationSet=ConfigurationSet",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "030e8250-b125-427f-8acc-47df3d6afbda"
            }
          ]
        },
        {
          "id": "10753c49-bc9f-44fd-a74f-341f86fe71c4",
          "name": "deleteConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSet?ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b219673-8fb3-4d2c-82f0-f1f045989836"
            }
          ]
        },
        {
          "id": "05dcb74f-37ec-45df-a8b5-f4857beb73be",
          "name": "describeConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationSet?ConfigurationSetAttributeNames.member.N=ConfigurationSetAttributeNames.member.N&ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e14ff337-833b-48de-a9be-fc9ff548a9fc"
            }
          ]
        },
        {
          "id": "807ca063-b9f9-4238-8e6f-1b5b60dc1925",
          "name": "listConfigurationSets",
          "request": {
            "url": "http://example.com/api/?Action=ListConfigurationSets?MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the configuration sets associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6090dbaf-de4a-4ef6-ac3d-de730b0fb13b"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "98cc63c1-2eaf-4385-abb2-18a7bd9770f2",
          "name": "createConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestination=EventDestination",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4602779f-36d9-4785-91b8-5bcc8e77661c"
            }
          ]
        },
        {
          "id": "fb4bad3e-fce5-40d3-9d9c-ce3649adf488",
          "name": "deleteConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestinationName=EventDestinationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be203811-0de1-4f58-84cd-33a4e4418708"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "70c37aa6-4c64-45ca-b580-88d306ce77bc",
          "name": "createReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptFilter?Filter=Filter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30f1f2be-72f5-40fb-9715-91a5752a69e4"
            }
          ]
        },
        {
          "id": "582381ec-2396-4efd-9a54-9f4ca650f5f8",
          "name": "deleteReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptFilter?FilterName=FilterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fbd0c5e-77fb-430a-9072-0fdc0a8c9575"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "8e187cff-f352-49bc-99a4-6c07642ea065",
          "name": "createReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRule?After=After&Rule=Rule&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "069874bd-1e71-472d-9397-d5051e02eeac"
            }
          ]
        },
        {
          "id": "5537bd62-879e-4ed8-885e-effe47f49439",
          "name": "deleteReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0513f710-0973-4f93-a2ca-bb4d590b5cdc"
            }
          ]
        },
        {
          "id": "f34ede9c-c569-4f51-9b3f-bd9a25ccfce5",
          "name": "describeReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f4a3ab7-38f0-45f3-8cdf-6c824385b0e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "7528fc33-ae46-4be1-825e-7bd53abf7217",
          "name": "deleteIdentity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentity?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified identity (an email address or a domain) from the list of verified identities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "034b0f2f-7f3e-40d6-8f71-d6f94e6610f4"
            }
          ]
        },
        {
          "id": "f669081a-0dad-4214-8f44-dd731a6de048",
          "name": "deleteIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentityPolicy?Identity=Identity&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified sending authorization policy for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12255deb-0df6-45ac-b6d6-835274a48b29"
            }
          ]
        },
        {
          "id": "7c1f4936-bb3f-485e-87db-6f3a413610f0",
          "name": "getIdentityDkimAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityDkimAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current status of Easy DKIM signing for an entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2cd5aea-5ac8-4995-94dd-10c1de9e13fb"
            }
          ]
        },
        {
          "id": "e47833c4-0e74-4157-b826-70f74b810658",
          "name": "getIdentityMailFromDomainAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityMailFromDomainAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the custom MAIL FROM attributes for a list of identities (email addresses and/or domains)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d20f3a92-2b72-42a9-9ada-e1853380671b"
            }
          ]
        },
        {
          "id": "187a09b8-6375-4e46-81e4-7a88aa9be9d9",
          "name": "getIdentityNotificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityNotificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of verified identities (email addresses and/or domains), returns a structure describing identity notification attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b96ccd6-54ea-434a-be93-d14f8229e203"
            }
          ]
        },
        {
          "id": "21198ad0-f6fb-4cf9-9fe8-fb2cd4139bc3",
          "name": "getIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPolicies?Identity=Identity&PolicyNames.member.N=PolicyNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the requested sending authorization policies for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ddc3fe1-b29c-4eba-b74d-e17d86bec579"
            }
          ]
        },
        {
          "id": "ec72738a-6ea8-46ab-adeb-80c03c8e2621",
          "name": "getIdentityVerificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityVerificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of identities (email addresses and/or domains), returns the verification status and (for domain identities) the verification token for each identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af729bf7-653d-4563-93b1-345b6930c5c3"
            }
          ]
        },
        {
          "id": "de14cc5a-72a0-46f8-a4af-354e8c799214",
          "name": "listIdentities",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentities?IdentityType=IdentityType&MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the identities (email addresses and domains) for your AWS account, regardless of verification status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c7791d5-5d2d-4a82-9de7-e8c0cec4e8b9"
            }
          ]
        },
        {
          "id": "2e5ec78d-6ce4-437d-ab67-62615bbcf548",
          "name": "listIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPolicies?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of sending authorization policies that are attached to the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce9a5d94-8168-4ef4-bb5e-ae87f7033d7f"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "fd0cc5b6-1d04-451d-b944-361ebd29210b",
          "name": "deleteVerifiedEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVerifiedEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified email address from the list of verified addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c16c047a-dd34-4dbb-b927-93467b22c5ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "9bb2b965-e694-413d-b021-fa2b008d6748",
          "name": "getSendQuota",
          "request": {
            "url": "http://example.com/api/?Action=GetSendQuota?Max24HourSend=Max24HourSend&MaxSendRate=MaxSendRate&SentLast24Hours=SentLast24Hours",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's current sending limits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65abf197-e88d-4d78-824f-f6ac2c30a510"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "7de7e29d-fd8a-4ea1-960e-b7fd78c22f08",
          "name": "getSendStatistics",
          "request": {
            "url": "http://example.com/api/?Action=GetSendStatistics?SendDataPoints.member.N=SendDataPoints.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's sending statistics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c700ca98-3e17-4b53-9a02-c83c8b52ec24"
            }
          ]
        }
      ]
    }
  ]
}