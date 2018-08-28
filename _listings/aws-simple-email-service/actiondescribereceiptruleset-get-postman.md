{
  "info": {
    "name": "AWS Simple Email Service API Describe Receipt Rule Set",
    "_postman_id": "eae5b0b1-83e1-44db-9e72-f62df9403567",
    "description": "Returns the details of the specified receipt rule set.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "c2890ce3-0072-47d3-b0fe-c4109a92be1c",
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
              "id": "61ff2d1d-f97d-46b7-9bb3-ff9ac2b36432"
            }
          ]
        },
        {
          "id": "9add0d09-29ea-496c-8bfa-d9d30e901206",
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
              "id": "f0f43901-6ef7-453c-b75c-4139a062ad52"
            }
          ]
        },
        {
          "id": "964f678b-77ba-46b3-ab5c-41feff5b9488",
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
              "id": "fcad4c68-ffce-4ea9-ae72-818a75175ed3"
            }
          ]
        },
        {
          "id": "4f5c1d0e-dfad-4972-8395-d8642a6c4f48",
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
              "id": "42ee84ea-1bea-4038-ad34-6e991c94ca08"
            }
          ]
        },
        {
          "id": "8a0da65a-bdff-4ddd-8940-4eafdeecc1f6",
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
              "id": "43d50c57-528e-499b-8755-d84c810e8324"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "f8db8611-9f7b-434f-b4ae-3f76763f230c",
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
              "id": "4630bb72-fef2-45c6-a157-21c8b9b32784"
            }
          ]
        },
        {
          "id": "b2e0872b-0993-4655-a959-be73fc27a9bd",
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
              "id": "272dd747-b247-4826-89bc-d6e6b4aea45a"
            }
          ]
        },
        {
          "id": "dc572703-1c92-4281-ba7e-6033adfd4bd8",
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
              "id": "803fdced-8133-4a71-96ce-8e9490a23093"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "fc1ce8c8-4fec-4e56-a552-baf1a2e0a84b",
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
              "id": "2bc33e8c-1c06-430f-b096-3a5b9616a059"
            }
          ]
        },
        {
          "id": "3213af21-7f1f-4fc0-bcc9-719aa35cdc80",
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
              "id": "e1f979ae-7cbc-4faa-8dba-89623cd1f3fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "7d986974-9584-4ff0-9f25-22a8e77045df",
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
              "id": "f442e6b8-1575-4786-a0c5-a709824c1aab"
            }
          ]
        },
        {
          "id": "0bc072d7-f34c-40db-81e8-3e966d979292",
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
              "id": "c53fbcd5-de1a-4a53-816f-bae69fb2543a"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "57cdfee1-a2aa-45e6-974b-0f24f535caf5",
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
              "id": "6e51fbd9-6702-4aa1-b34e-b0da758475ca"
            }
          ]
        },
        {
          "id": "147a5113-f33e-497e-8bb1-2a712b01c731",
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
              "id": "fd66e6ed-5e45-4229-ae15-74edabb4b03b"
            }
          ]
        },
        {
          "id": "84ee83b1-f87b-4b04-b836-1731464bc923",
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
              "id": "847e1b8a-6983-4cae-a49e-5d60cbbf9383"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "83209e62-adce-46a5-9aa0-584f29b9add1",
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
              "id": "e4e4ca58-39df-4875-a040-0ed12144cfdf"
            }
          ]
        },
        {
          "id": "591d537d-d2d2-4e56-b6e4-558f20ff7705",
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
              "id": "9e558370-8567-45b3-a4b4-197b0ee9822e"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "b85a3407-3e04-49ec-bc13-0faeb80fc4b3",
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
              "id": "1ac74c4f-fe90-49d8-88e8-48776887a9c6"
            }
          ]
        }
      ]
    }
  ]
}