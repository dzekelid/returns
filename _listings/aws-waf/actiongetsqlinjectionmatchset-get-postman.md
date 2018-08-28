{
  "info": {
    "name": "AWS WAF API Get Sql Injection Match Set",
    "_postman_id": "d3cadaff-7883-48ed-b0e4-74a9067e5f60",
    "description": "Service: AWS WAFReturns the.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web ACL",
      "item": [
        {
          "id": "60a1529b-fac2-49a9-a9a2-4bee5136ccbc",
          "name": "associateWebACL",
          "request": {
            "url": "http://example.com/api/?Action=AssociateWebACL?ResourceArn=ResourceArn&WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalAssociates a web ACL with a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a0f26db-c1a2-44c5-b7ab-b4980aaf4b21"
            }
          ]
        },
        {
          "id": "1a98a226-87bc-4745-ac78-1a2aabf6943e",
          "name": "createWebACL",
          "request": {
            "url": "http://example.com/api/?Action=CreateWebACL?ChangeToken=ChangeToken&DefaultAction=DefaultAction&MetricName=MetricName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a WebACL, which contains the Rules that identify the CloudFront web requests that you want to allow, block, or count."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48823599-7f3b-49b3-858a-8d8ac0384fce"
            }
          ]
        },
        {
          "id": "475773da-9710-4145-a30a-6b05bde3b8ca",
          "name": "deleteWebACL",
          "request": {
            "url": "http://example.com/api/?Action=DeleteWebACL?ChangeToken=ChangeToken&WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88622742-2162-40a3-bd91-f9ff3c374e0d"
            }
          ]
        },
        {
          "id": "601230bc-0c6f-4089-8c12-f031c413d5c3",
          "name": "disassociateWebACL",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateWebACL?ResourceArn=ResourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalRemoves a web ACL from the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee94d673-10de-45bd-93db-a32019a09104"
            }
          ]
        }
      ]
    },
    {
      "name": "Byte Match Set",
      "item": [
        {
          "id": "6328faf1-2d64-419c-a81d-bacb93874791",
          "name": "createByteMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateByteMatchSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a ByteMatchSet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10bd606d-a152-4d4f-bb00-5f99f0143542"
            }
          ]
        },
        {
          "id": "a29104d6-ba76-4fc4-b446-0351a97fd445",
          "name": "deleteByteMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteByteMatchSet?ByteMatchSetId=ByteMatchSetId&ChangeToken=ChangeToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b9f9c2b-112d-4c86-8ea7-452485fdbe9f"
            }
          ]
        },
        {
          "id": "769aa1a0-80b2-4b22-82a4-44a804c75978",
          "name": "getByteMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=GetByteMatchSet?ByteMatchSetId=ByteMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba84b310-10f1-4ab9-8ecd-9c8620ad8901"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Sets",
      "item": [
        {
          "id": "df76218b-6887-4153-8287-65f5e08e910b",
          "name": "createIPSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateIPSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6777aed1-25d5-4888-b9d3-f7201431a276"
            }
          ]
        },
        {
          "id": "96b07ea3-46f9-4ce5-a737-07852646d81b",
          "name": "deleteIPSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIPSet?ChangeToken=ChangeToken&IPSetId=IPSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b6fcb21-fa75-4a2e-bf1a-ef720c5e2acb"
            }
          ]
        },
        {
          "id": "7f3e6509-a23e-4991-a361-82d539b34504",
          "name": "getIPSet",
          "request": {
            "url": "http://example.com/api/?Action=GetIPSet?IPSetId=IPSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8b2a4aa-e367-4ca9-a9bb-926951bc7b7e"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "0eed4cd0-dc09-4a81-a4c2-8ce1b3e8195b",
          "name": "createRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateRule?ChangeToken=ChangeToken&MetricName=MetricName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a Rule, which contains the IPSet objects, ByteMatchSet objects, and \n\t\t\tother predicates that identify the requests that you want to block."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9dcb4a1a-7d6e-42fe-8fc6-75e839f4884f"
            }
          ]
        },
        {
          "id": "1d31049d-732e-4025-94be-db4120e5d036",
          "name": "deleteRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRule?ChangeToken=ChangeToken&RuleId=RuleId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b1a5aba-62ba-4394-b6d2-1badfcaba9b7"
            }
          ]
        },
        {
          "id": "f1658aaa-7446-409a-979a-16a51f6c3939",
          "name": "getRule",
          "request": {
            "url": "http://example.com/api/?Action=GetRule?RuleId=RuleId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cb13860-7342-4a17-bfe1-6c5ab077cf90"
            }
          ]
        }
      ]
    },
    {
      "name": "Size Constraint Set",
      "item": [
        {
          "id": "de2fc5df-491f-449c-880c-54af78366f12",
          "name": "createSizeConstraintSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateSizeConstraintSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a SizeConstraintSet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f5a0ebe-fae0-4631-bc4b-9a7bc619f0ca"
            }
          ]
        },
        {
          "id": "bc70dc32-d0ad-4ce6-bf8f-8bc7c805285d",
          "name": "deleteSizeConstraintSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSizeConstraintSet?ChangeToken=ChangeToken&SizeConstraintSetId=SizeConstraintSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3107a7d3-e3ca-4d15-84b0-9e5630c67230"
            }
          ]
        },
        {
          "id": "a5374751-6f7b-4865-b134-253a05b7fc39",
          "name": "getSizeConstraintSet",
          "request": {
            "url": "http://example.com/api/?Action=GetSizeConstraintSet?SizeConstraintSetId=SizeConstraintSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c6642b3-72f3-41f5-9d20-d227239aaca0"
            }
          ]
        }
      ]
    },
    {
      "name": "SQL Injection Match Set",
      "item": [
        {
          "id": "5d6e3f10-da8d-441f-92ee-3d3507228b71",
          "name": "createSqlInjectionMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateSqlInjectionMatchSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7a8e942-ba34-4fdc-ad9c-a81b3c1e67d4"
            }
          ]
        },
        {
          "id": "841382c7-d16d-423b-a55d-0e1c3951d985",
          "name": "deleteSqlInjectionMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSqlInjectionMatchSet?ChangeToken=ChangeToken&SqlInjectionMatchSetId=SqlInjectionMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fcf4d6d-8591-4715-a156-c6c39998568d"
            }
          ]
        },
        {
          "id": "0ce85930-9ff6-434a-8744-5a5ace809e56",
          "name": "getSqlInjectionMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=GetSqlInjectionMatchSet?SqlInjectionMatchSetId=SqlInjectionMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "caf7091b-0ded-4466-8b5c-d0e71ab74023"
            }
          ]
        }
      ]
    },
    {
      "name": "XSS Match Set",
      "item": [
        {
          "id": "fc3ff50a-778b-4e76-8687-7e6332181096",
          "name": "createXssMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateXssMatchSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e109516e-d9fd-48c2-a0fb-a8a670c7b302"
            }
          ]
        },
        {
          "id": "18422357-bb35-4dd0-a4e0-af444214336b",
          "name": "deleteXssMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteXssMatchSet?ChangeToken=ChangeToken&XssMatchSetId=XssMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "475876a9-6e2d-498d-ac2f-3898214dc484"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Token",
      "item": [
        {
          "id": "6aa87610-f728-4251-80b5-18c2a2af879e",
          "name": "getChangeToken",
          "request": {
            "url": "http://example.com/api/?Action=GetChangeToken?ChangeToken=ChangeToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFWhen you want to create, update, or delete AWS WAF objects, get a change token and include the change token in the create, update, or delete request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6939590c-a896-4808-853f-f17d020321cb"
            }
          ]
        },
        {
          "id": "6d4dbd75-0e2b-44e8-b396-e0f40cbcf7ca",
          "name": "getChangeTokenStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetChangeTokenStatus?ChangeToken=ChangeToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the status of a ChangeToken that you got by calling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c292cdb0-b291-489c-895a-74fe52abef7e"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "4286b584-d443-40b5-a376-910275678a35",
          "name": "getSampledRequests",
          "request": {
            "url": "http://example.com/api/?Action=GetSampledRequests?MaxItems=MaxItems&RuleId=RuleId&TimeWindow=TimeWindow&WebAclId=WebAclId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFGets detailed information about a specified number of requests--a sample--that AWS WAF randomly selects from among the first 5,000 requests that your AWS resource received during a time range that you choose."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64f8f80b-3a8c-4a91-976f-1a2320105376"
            }
          ]
        }
      ]
    }
  ]
}