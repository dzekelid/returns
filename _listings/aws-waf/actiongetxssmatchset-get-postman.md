{
  "info": {
    "name": "AWS WAF API Get Xss Match Set",
    "_postman_id": "420dbc09-f3ef-4607-8d82-26202612254a",
    "description": "Service: AWS WAFReturns the.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web ACL",
      "item": [
        {
          "id": "634f274a-1280-4147-a467-8b84163bf380",
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
              "id": "a00e43f6-5c67-4537-83fd-6f523cc0c271"
            }
          ]
        },
        {
          "id": "b04abc60-c276-4529-998b-276233713c6e",
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
              "id": "63f21621-90de-4e60-8467-7fc26192761e"
            }
          ]
        },
        {
          "id": "90312af4-4639-472d-a0af-18f50d507b57",
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
              "id": "ec3734c3-2c7c-4783-a647-a8502c33af95"
            }
          ]
        },
        {
          "id": "123aa09d-30ed-4aa5-a764-a048dc293859",
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
              "id": "24440f72-86f9-4d41-ac1d-512771128545"
            }
          ]
        },
        {
          "id": "c53ab292-69e8-4e46-b3e6-999cecd6a4df",
          "name": "getWebACL",
          "request": {
            "url": "http://example.com/api/?Action=GetWebACL?WebACLId=WebACLId",
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
              "id": "c5a8d0c7-2f30-4484-bd8b-dc4f9134f7ed"
            }
          ]
        },
        {
          "id": "c498b9f5-e256-40ea-8212-08df79451ec7",
          "name": "getWebACLForResource",
          "request": {
            "url": "http://example.com/api/?Action=GetWebACLForResource?ResourceArn=ResourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalReturns the web ACL for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3842c7d2-4947-47bf-bf9e-3628aedd6836"
            }
          ]
        }
      ]
    },
    {
      "name": "Byte Match Set",
      "item": [
        {
          "id": "e5802e15-41a6-4016-a6e5-869c8abc4565",
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
              "id": "e18b942d-3c1e-4d16-8d96-89c166584c1e"
            }
          ]
        },
        {
          "id": "cbcdc05d-6af8-4504-82f2-4df9efbb12cf",
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
              "id": "9dda72e0-9097-4e9e-916c-cf6284ffcb9f"
            }
          ]
        },
        {
          "id": "4c1550cb-74b2-4f4c-903b-5f100b2d7c8c",
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
              "id": "11645241-c0b6-4b8e-981e-93e3ece1e589"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Sets",
      "item": [
        {
          "id": "5a022562-5e1f-4ee6-a59b-676259cbbbd3",
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
              "id": "84d3e072-4015-46b7-b643-8050496ec162"
            }
          ]
        },
        {
          "id": "ff4adafa-206b-48ba-be6a-449c63c70dd3",
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
              "id": "de65b640-d322-420c-90c7-de6ecd5099a3"
            }
          ]
        },
        {
          "id": "43482e91-b21c-4b0c-aca7-9c9f0d366865",
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
              "id": "e1932e89-8f61-44d2-a39a-48c57fef5b20"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "b174b9f3-e374-4825-863f-15bad5ceff58",
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
              "id": "53df91aa-4b0f-49bb-a191-589818fe6202"
            }
          ]
        },
        {
          "id": "f221f67e-5b48-4add-8656-30933586a7b5",
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
              "id": "f9516c25-990c-42b8-8855-55674e02a73d"
            }
          ]
        },
        {
          "id": "4b208f65-aa31-4532-8ce9-dbfcd3fc26d9",
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
              "id": "10e37aac-f999-4602-821a-deac062b5f97"
            }
          ]
        }
      ]
    },
    {
      "name": "Size Constraint Set",
      "item": [
        {
          "id": "27a330df-4a98-4e0c-a62d-8578127ebc7e",
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
              "id": "b1a96f25-dc9e-45ea-888b-614673389c79"
            }
          ]
        },
        {
          "id": "6c6822b8-6548-4481-b3cc-cac8f1adb057",
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
              "id": "0cd4ed89-a44a-4bb4-95f9-1c8cbbc3fbd4"
            }
          ]
        },
        {
          "id": "38963b9b-cd66-489c-a12e-0a4d8d30748e",
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
              "id": "29c769fa-86a4-4688-a520-408fa622c8d9"
            }
          ]
        }
      ]
    },
    {
      "name": "SQL Injection Match Set",
      "item": [
        {
          "id": "0d6ee12e-c4d2-4f8d-b603-11f89bac86dd",
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
              "id": "033ef8d5-2d96-42e2-80dc-a0a269233f1a"
            }
          ]
        },
        {
          "id": "e58973e2-2746-46dc-9658-5429222cfa6c",
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
              "id": "8c47cbc0-3bcc-4bfb-8cef-9f31db611231"
            }
          ]
        },
        {
          "id": "73f2c454-0abf-4485-a619-7bf9673b8cda",
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
              "id": "c4de1c9e-1001-44a1-a1c2-5ed9c7cc8bb8"
            }
          ]
        }
      ]
    },
    {
      "name": "XSS Match Set",
      "item": [
        {
          "id": "b6168b8a-5007-4420-a6e6-6ccde65ed8a3",
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
              "id": "28233fba-0953-4757-8d31-86c3926ad973"
            }
          ]
        },
        {
          "id": "34ddc6d8-1318-4b29-92ef-cf63d78b462c",
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
              "id": "4471b82d-ec74-4983-bac4-ffb439f3c751"
            }
          ]
        },
        {
          "id": "43cae573-a2dd-430c-9409-a08aa1d3fec5",
          "name": "getXssMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=GetXssMatchSet?XssMatchSetId=XssMatchSetId",
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
              "id": "5187a186-466c-4637-9c64-f15eefa2886c"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Token",
      "item": [
        {
          "id": "55216609-bd46-4b9d-916c-0163c7c9fee5",
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
              "id": "7f5acf0c-b7cf-4a22-9218-96ce1b51e2cf"
            }
          ]
        },
        {
          "id": "7c301dfc-0a55-47d0-83dd-dd7f64745ee3",
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
              "id": "93de0f23-9693-4cdf-9b78-2a0a263db2bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "d5b0056a-ec1d-4c0f-9ba0-7525f0a83cee",
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
              "id": "346720d1-40b0-4d7e-9adc-4d0f9731770b"
            }
          ]
        }
      ]
    }
  ]
}