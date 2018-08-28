{
  "info": {
    "name": "AWS WAF API Get Byte Match Set",
    "_postman_id": "04630b23-f5ed-4357-b3eb-ef3eb982c292",
    "description": "Service: AWS WAFReturns the.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web ACL",
      "item": [
        {
          "id": "902e3bb6-4ee1-4ac0-bdc4-2bbbc2b21579",
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
              "id": "bc0746f2-30fa-4da1-b51b-fd4108f2c32c"
            }
          ]
        },
        {
          "id": "6114b6cd-a5dc-4afc-8de5-08cf716ae83a",
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
              "id": "c320e805-8f75-48b1-a98a-d64c88dabaf5"
            }
          ]
        },
        {
          "id": "0ba0b974-b236-4bff-8f83-dd6d9290174a",
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
              "id": "90bbc156-551b-4c19-858b-0fa5bf97a902"
            }
          ]
        },
        {
          "id": "e3aadd82-e2c1-4a1b-8416-a1d988052df5",
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
              "id": "13a01185-42bb-4787-aa5c-acaf60eb7ba6"
            }
          ]
        }
      ]
    },
    {
      "name": "Byte Match Set",
      "item": [
        {
          "id": "f43b8638-be2f-4b65-b272-95c4cceb1bc2",
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
              "id": "07212d28-889d-42b7-9964-f3136326c0b4"
            }
          ]
        },
        {
          "id": "8c5a77d0-348d-42d9-94e2-c58902ab3e0e",
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
              "id": "48743b21-6b5f-4634-9846-39e961c53aa1"
            }
          ]
        },
        {
          "id": "5b11f241-ea3b-4c27-8ef2-cb5dea4eb2b6",
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
              "id": "2d875dd6-f83c-4ab9-86db-bd15b83ba5e9"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Sets",
      "item": [
        {
          "id": "42b9b0bc-2164-4820-93d6-dc3f3d732b01",
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
              "id": "6d43c65d-d712-4225-a382-5ffb310fa56f"
            }
          ]
        },
        {
          "id": "31ed4430-796a-48c0-9e22-5e39399cff6f",
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
              "id": "9446f502-fd5f-459b-9bf8-1ece16d79737"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "68a13496-5c6b-4d4b-b7fb-e2c0d827dea8",
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
              "id": "8ff3cb7d-4327-45b2-a9a3-390ea64619a8"
            }
          ]
        },
        {
          "id": "eac4ef26-c731-49fa-938c-ea136159b43b",
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
              "id": "c7ea3811-007f-43cc-9545-4b762d9134b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Size Constraint Set",
      "item": [
        {
          "id": "eac6bfb9-bc29-4c81-b584-de4f70b4fb37",
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
              "id": "c2ec6b59-b97e-4c16-9d6c-be6dc262eee1"
            }
          ]
        },
        {
          "id": "ee34c361-e469-4877-a194-d56358471b29",
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
              "id": "24636875-c702-4fce-8e89-d73057107eb3"
            }
          ]
        }
      ]
    },
    {
      "name": "SQL Injection Match Set",
      "item": [
        {
          "id": "861e5479-8255-40e4-a5e9-2c897a5092e0",
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
              "id": "4cde4687-51ef-4138-a552-5e153ac052aa"
            }
          ]
        },
        {
          "id": "00041f0a-a4ff-4092-9843-a52e18c3f047",
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
              "id": "22730de5-c407-4044-83aa-ba6e42c8ec75"
            }
          ]
        }
      ]
    },
    {
      "name": "XSS Match Set",
      "item": [
        {
          "id": "28241f35-8f47-480f-8225-f00829f84d36",
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
              "id": "46d5e7ec-c2e0-4ee1-8aa4-6ca221d8f689"
            }
          ]
        },
        {
          "id": "e10704ae-1124-46e9-870b-0089260e7011",
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
              "id": "2e908314-6928-462c-a92c-fa3ff60b81b9"
            }
          ]
        }
      ]
    }
  ]
}