{
  "info": {
    "name": "AWS Simple Email Service API Describe Active Receipt Rule Set",
    "_postman_id": "7839d3bd-394f-4337-8c71-28067c38e1bd",
    "description": "Returns the metadata and receipt rules for the receipt rule set that is currently active.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "3b081e0d-fa0a-43a9-be3f-0213fe3faaca",
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
              "id": "817c6d37-7534-462c-b955-a3b684a2660b"
            }
          ]
        },
        {
          "id": "7a49cca3-c197-4576-a31e-47b93b376ca7",
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
              "id": "ce4a21f9-51e4-4e27-982f-09cdd3b4617f"
            }
          ]
        },
        {
          "id": "8d10c771-ce38-472b-83a3-6b0d26e2be27",
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
              "id": "65e2715d-a5f6-4512-b608-1e1d9d36d1ff"
            }
          ]
        },
        {
          "id": "ad9b64f8-8179-4876-bfc0-a89b5ed3d03f",
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
              "id": "b5f63330-7fb9-4f7f-a780-d7b15a711eb9"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "4b124b3f-1f48-4d48-b0c2-6d2e6c37e942",
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
              "id": "40c2bb2b-3786-42e5-ba94-b57cb39d27ea"
            }
          ]
        },
        {
          "id": "c428feba-53a3-4444-9eca-717c152471e7",
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
              "id": "f494aad2-d09b-4e36-951b-713304c6f105"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "52438d09-dd27-43e4-a57f-57af1946d4cb",
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
              "id": "fd9107eb-61ca-4763-b262-ea2b53a2ea47"
            }
          ]
        },
        {
          "id": "b2988f4b-58e7-4242-a067-492dddfdd113",
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
              "id": "7d2ab526-ca6d-446b-b1c8-86e3a7e7ca1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "0d12993a-b079-4869-9e95-d29df0a2f671",
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
              "id": "66cbb8ac-7cf7-4154-9608-82a6e23b0e3e"
            }
          ]
        },
        {
          "id": "1edb8147-92d8-4883-a039-bd51cde84f40",
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
              "id": "5eb15d2c-b96f-4cad-bf75-688fe4ec961a"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "ebc182d3-3739-4d28-8aaa-6efed6bbf038",
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
              "id": "3f1fc581-7429-44eb-aeef-8e23583192bf"
            }
          ]
        },
        {
          "id": "acb63c7a-cada-4288-b6d2-828aedd0146c",
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
              "id": "661afcff-1cd0-4362-b8ad-7fe6de366cb7"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "b1cf7f8a-a8ed-4753-bf4f-54074d6cb046",
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
              "id": "63f6be03-22fe-4848-aa9c-fde499aaaff7"
            }
          ]
        },
        {
          "id": "9086fef7-e86d-4f00-9448-923830376bac",
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
              "id": "46cfefe7-d31c-4e30-9612-888bc94ba202"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "f858bdd7-8617-4260-aa90-e112484c719b",
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
              "id": "3dde3379-5866-4fe7-8403-f77c5466950a"
            }
          ]
        }
      ]
    }
  ]
}