{
  "info": {
    "name": "AWS Simple Email Service API List Identities",
    "_postman_id": "f3da6947-7a1e-41ce-8f58-084ae93edb1b",
    "description": "Returns a list containing all of the identities (email addresses and domains) for your AWS account, regardless of verification status.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "c3a6cb17-1927-47c5-811b-56e0df62e47d",
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
              "id": "c3e2e61b-6618-43b1-b7d4-f5bff678629e"
            }
          ]
        },
        {
          "id": "608bc1ca-dda4-4df2-96f4-4714ea238565",
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
              "id": "78ed94e5-3c59-4bfb-8f25-90acf137b5d6"
            }
          ]
        },
        {
          "id": "ca2b1a62-1690-494c-8380-f272bfb3ead7",
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
              "id": "cfd58987-7f97-49cc-bd81-2948986398e4"
            }
          ]
        },
        {
          "id": "5efaeb00-6e44-4e69-ac40-8f306999e188",
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
              "id": "4439e804-2873-4c69-979c-f68a892fbdbc"
            }
          ]
        },
        {
          "id": "499afb39-6e68-442d-8619-476a06311579",
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
              "id": "5e0b8987-f60c-4651-822e-8d7ca2fd04b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "433301c9-5b95-4e65-9235-58cc96937f60",
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
              "id": "db5a8270-b12b-4b31-8f01-bf1b1f0cecf9"
            }
          ]
        },
        {
          "id": "0d3fdbcb-fac9-45a9-a3d0-6de7246402bd",
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
              "id": "e8cd143d-cbca-472c-a456-b5b7b9ce726a"
            }
          ]
        },
        {
          "id": "79840edc-ce2a-42bf-af2a-04a7a88ac804",
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
              "id": "75eb2da0-4944-4159-965e-7710539e61b7"
            }
          ]
        },
        {
          "id": "57565291-2415-4ad1-b969-33c573d33362",
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
              "id": "4054d847-a1f4-4516-abc1-1b961072e8af"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "6d6f0504-7d0b-4a09-abdc-a3b6c166af08",
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
              "id": "12f4f5ea-63e6-4411-83eb-7e92195fc7a0"
            }
          ]
        },
        {
          "id": "31dbc321-ca22-4232-9f35-dda8a88919b8",
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
              "id": "297eaf72-996c-4ee2-8722-56d9b48319c6"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "a3432d07-5018-4941-a01b-890634d85900",
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
              "id": "27956d67-984b-486e-b40a-bcefd42b0c2f"
            }
          ]
        },
        {
          "id": "bfd25485-0021-4ab4-870c-b42e37671557",
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
              "id": "332d41ea-d388-4518-81ae-3000c75d558d"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "b4b93583-dd19-4522-86b0-322281125cb0",
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
              "id": "c8d5ff97-21c2-4e32-a409-8c06891c9b57"
            }
          ]
        },
        {
          "id": "0cfe6cac-cf61-4f9f-8fc2-fdbf40753f40",
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
              "id": "ea8efbce-dd0d-455d-ae44-619bedfc5a4d"
            }
          ]
        },
        {
          "id": "c67f8d88-6082-4f99-964e-b8e2a3f70113",
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
              "id": "a12e8bd9-71a0-451f-a6cb-84cc4830d66a"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "dfee9acb-4d78-489d-8495-68f018c7332c",
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
              "id": "04d19071-9c56-40af-954d-b4b3628bfb21"
            }
          ]
        },
        {
          "id": "430e1f1c-705a-4b6a-a71c-542238d40d9d",
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
              "id": "c6933040-f9b8-4d3d-8e0d-a18f2e678648"
            }
          ]
        },
        {
          "id": "59b08568-46fb-4d82-9ba1-0f86b2350d57",
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
              "id": "1d4568d9-57c5-497a-a220-c67e710c1da7"
            }
          ]
        },
        {
          "id": "a49b5167-e44f-45bc-95bd-29a5cf6b7307",
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
              "id": "0ebf91c3-dbf0-4243-a441-33b2562a3f1e"
            }
          ]
        },
        {
          "id": "140ee18e-8ae9-41ae-899c-07c4f9475d67",
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
              "id": "04d368b0-543a-4199-87a2-782db241fae1"
            }
          ]
        },
        {
          "id": "6584ceb6-8120-4756-8ca4-c20af5142fe7",
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
              "id": "5e3f421c-8031-46d0-b311-9729e42cde9f"
            }
          ]
        },
        {
          "id": "f15bf6bd-c19a-4acc-a83b-e35eb4ec0891",
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
              "id": "38bb720f-bcbd-4a80-8fdb-c64b705b8771"
            }
          ]
        },
        {
          "id": "aa9ea212-a509-4edf-a177-d4be20d716f5",
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
              "id": "aa3caced-ad9a-475c-b38b-0698f3575daf"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "76633832-cd6f-4dc1-addc-778f909125fa",
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
              "id": "2b6f94b7-8a51-4b5a-8fc4-e269a5f5b0c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "dcc653b6-e7c7-40dd-8729-5d0aa19d2cea",
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
              "id": "55df62e4-7cb6-442f-85c9-f92dea584ee5"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "61bad4d7-c571-450e-af31-ddc96ea47b31",
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
              "id": "1b4823f6-6387-4fcf-a920-5a740174e507"
            }
          ]
        }
      ]
    }
  ]
}