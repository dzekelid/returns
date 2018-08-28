{
  "info": {
    "name": "AWS WAF API Get IP Set",
    "_postman_id": "5552783c-0f72-44bf-b6e3-d1cb1d613106",
    "description": "Service: AWS WAFReturns the.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web ACL",
      "item": [
        {
          "id": "288e8462-8eb7-46fa-b0b4-2d115ebeef22",
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
              "id": "0e7dee3b-351b-4b44-b03e-267afd5fa993"
            }
          ]
        },
        {
          "id": "b7db27fa-e6cc-424a-9dfe-7b990e6af683",
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
              "id": "75061f8d-f9e2-461d-b3da-242b09762566"
            }
          ]
        },
        {
          "id": "c6b90a6f-17ba-4d6c-b248-3d8eccafc0c9",
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
              "id": "408f2f37-fcc4-43f8-9393-ba2eb87c23fb"
            }
          ]
        },
        {
          "id": "fe020b7b-fc0f-41cf-b4b7-3c852e1f1efe",
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
              "id": "d7442cd0-3d16-47da-9c08-968f3fe3f5f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Byte Match Set",
      "item": [
        {
          "id": "fb1327b0-7ff9-4e94-a6b6-5fcf5ce87371",
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
              "id": "3fb3a29a-6419-441a-9f3d-3278e4e86e1b"
            }
          ]
        },
        {
          "id": "5fd1dbaf-707e-4d79-b6c8-82142773ad53",
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
              "id": "16de855c-1a9b-4093-b5c1-ad8916daa8e2"
            }
          ]
        },
        {
          "id": "fe1a078e-fdca-4f1e-9e13-a7b8037f30fa",
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
              "id": "b57c0c10-420f-491d-8015-d1e3e1304e39"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Sets",
      "item": [
        {
          "id": "bdc4930b-0578-4c44-9387-cf7d7457233e",
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
              "id": "8e842a9e-da13-4a2c-8ba9-20e052b62512"
            }
          ]
        },
        {
          "id": "56fcb658-15b1-43f9-9531-c23dea4ce015",
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
              "id": "e33bb185-e3e4-412a-9795-2be5de873f05"
            }
          ]
        },
        {
          "id": "666eb933-1ac2-4feb-812d-5e1a403550a9",
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
              "id": "a2b478a9-d828-40d7-90c4-dfe12d5aede1"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "fb8ae226-2d53-47de-8cc4-1f22939ab750",
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
              "id": "310c33a1-d5a6-4204-8eb8-d238fa43f39e"
            }
          ]
        },
        {
          "id": "037830ef-498b-49ba-ba7d-58fd9eb0bb49",
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
              "id": "d82912b1-8483-4616-89c6-887efcd0e8b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Size Constraint Set",
      "item": [
        {
          "id": "fe6472fb-ee2a-44f4-b2c3-5fd041f2776b",
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
              "id": "132e90f0-9ffc-4b36-8ad5-5978a57a3986"
            }
          ]
        },
        {
          "id": "e25dcfdd-200c-4695-8c1d-3ce2fb37e583",
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
              "id": "67dbf876-fb3a-496f-9402-2aa58f2d6329"
            }
          ]
        }
      ]
    },
    {
      "name": "SQL Injection Match Set",
      "item": [
        {
          "id": "ba84e981-7682-4ebd-a2e8-e30d78d4e4bf",
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
              "id": "adbf0d4b-21b1-438c-b3d1-a35c7496d90a"
            }
          ]
        },
        {
          "id": "88979573-c3b5-4d6f-a462-35ecc9d0cf84",
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
              "id": "e6fc7183-1f64-45b0-b9ed-e1d6dd967f51"
            }
          ]
        }
      ]
    },
    {
      "name": "XSS Match Set",
      "item": [
        {
          "id": "886fcdbe-857f-482d-86b9-502239c7a1e8",
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
              "id": "43715d45-4ad2-4d73-8bf9-ceba88a19d97"
            }
          ]
        },
        {
          "id": "321665dc-c8df-4c0b-8f9b-790e0af4e912",
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
              "id": "863cfe9b-1c47-410c-b5cf-530039c7050e"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Token",
      "item": [
        {
          "id": "b3fd9322-52da-4fed-b715-3ce0ab720e29",
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
              "id": "c21c9004-5d88-4692-92a3-24ce4491c4fd"
            }
          ]
        },
        {
          "id": "6143361f-916f-44f4-9e9b-7ae8a98963f4",
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
              "id": "cfe415e5-4a5f-4e5b-bce5-3e21e5c94820"
            }
          ]
        }
      ]
    }
  ]
}