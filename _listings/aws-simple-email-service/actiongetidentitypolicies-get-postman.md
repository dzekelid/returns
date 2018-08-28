{
  "info": {
    "name": "AWS Simple Email Service API Get Identity Policies",
    "_postman_id": "46ba3fd5-1b16-4724-aa2d-6241c890c722",
    "description": "Returns the requested sending authorization policies for the given identity (an email address or a domain).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "f29f3466-f58e-4d09-9746-394e76a3d498",
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
              "id": "ae2edb10-dd7d-43bc-8bdd-f5c0eea60dac"
            }
          ]
        },
        {
          "id": "e96158c9-e938-4c2e-8aa3-0eacb97a166a",
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
              "id": "46c2055f-14e8-4629-900e-9d6db4b8b509"
            }
          ]
        },
        {
          "id": "e2756458-fa9d-4473-b5e7-f891574efe34",
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
              "id": "0d446d32-0f15-47ce-9bb8-0a2a50090386"
            }
          ]
        },
        {
          "id": "b36dc539-ad75-4377-9aa8-90ae12588c84",
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
              "id": "25c826a0-7478-43c7-ab5a-6bfc28d036fa"
            }
          ]
        },
        {
          "id": "522d6ef7-3b7d-4f13-9787-d09fbcd48ac0",
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
              "id": "dc427f69-10d0-4303-9ac7-5f87abb239dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "bd4eb969-9dea-42fd-9e43-25cc3f329e07",
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
              "id": "c7977fe9-e9ef-4bf8-8a11-c93a03889c68"
            }
          ]
        },
        {
          "id": "34569ae0-d44d-49aa-a5ab-09f40e3c39e2",
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
              "id": "b16d9c52-ffcb-4c0e-8219-2f708b4cecf2"
            }
          ]
        },
        {
          "id": "a16acd06-f335-4a99-9515-24095010eb49",
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
              "id": "3f1ffbcc-eeb3-4ca4-b763-5d96fd6faba5"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "dc7d4d10-30e9-4aeb-a8a7-427a2d36cd21",
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
              "id": "4b69c2f8-c632-4c0d-8bb3-793080e22ec8"
            }
          ]
        },
        {
          "id": "1bd0806e-cb9e-4be9-8815-3ca1dd794f7e",
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
              "id": "7e32d494-b5e5-4227-9a27-041c40cbad8f"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "83ff2bc6-5c3a-4417-bae5-32c7cf289c9c",
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
              "id": "60920b07-7814-4518-b072-fce9a03c747e"
            }
          ]
        },
        {
          "id": "979e2768-b371-453b-9814-5a5ff90e4c42",
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
              "id": "b685d1fb-f0bd-44a2-b42e-00e409b3035b"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "4210570c-eb27-40b9-8653-4e8b378b953c",
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
              "id": "3b548f48-cd13-4b4d-a9cf-04a10c20ba92"
            }
          ]
        },
        {
          "id": "bd027acf-0dea-4169-97ba-725ad5dd3958",
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
              "id": "e190c15f-7e3f-4b77-91fe-a7614336d978"
            }
          ]
        },
        {
          "id": "964afc1b-f619-4c05-a01d-e37cb3874183",
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
              "id": "2b06f69b-e00e-4267-b815-35f441b95b28"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "33d870b7-c725-40d9-98d1-bf60066d4fd0",
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
              "id": "1fa7f2a7-f6f6-4533-91f4-afb7a86a4eb8"
            }
          ]
        },
        {
          "id": "db48ee82-3d86-4ace-b6a6-bfed59950de8",
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
              "id": "67fa7336-9ffb-4969-8ac7-b002e9fcd8dc"
            }
          ]
        },
        {
          "id": "4a53620c-7ede-4775-8859-33147325ec40",
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
              "id": "f26b0664-8389-4592-96f2-1589512f9345"
            }
          ]
        },
        {
          "id": "1112b5f8-38c4-4270-b700-81cfab4678a3",
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
              "id": "ef2ee8f1-5d47-4ee6-b71d-987e617a728c"
            }
          ]
        },
        {
          "id": "a33cc668-584a-407f-aa64-9a5ebece5629",
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
              "id": "27f23578-4292-4314-bc1b-17f3a0a6a337"
            }
          ]
        },
        {
          "id": "2784b18a-27a3-4604-ba2f-fa2e18a891b0",
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
              "id": "7c24712e-5cdc-4c59-9b29-83e587b2d960"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "5ca66c2b-50ca-41de-9598-0215a6b1213f",
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
              "id": "ee02ac7b-1b65-426b-9b9c-a394bcb72599"
            }
          ]
        }
      ]
    }
  ]
}