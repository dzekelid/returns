{
  "info": {
    "name": "AWS WAF API Get Size Constraint Set",
    "_postman_id": "4c80e99d-6c72-4708-9770-92c7f772ae1e",
    "description": "Service: AWS WAFReturns the.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web ACL",
      "item": [
        {
          "id": "3bffc373-e7ea-4dc5-9563-8f7485c4f8cd",
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
              "id": "ac8b31d4-3376-469d-aec0-22db74c65507"
            }
          ]
        },
        {
          "id": "4ea0605a-194d-4e39-8983-42e93867fb93",
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
              "id": "b4a6ce5e-2112-49da-86d5-f896aa761204"
            }
          ]
        },
        {
          "id": "0d3e8783-57de-4219-a01f-e32da03fefe4",
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
              "id": "08b0ee5a-53f5-43df-95a4-653b50510f6e"
            }
          ]
        },
        {
          "id": "4cb93f0e-835e-42cb-a164-a3538a47524a",
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
              "id": "a7c8d322-ed70-4768-a740-1b981ed1baad"
            }
          ]
        }
      ]
    },
    {
      "name": "Byte Match Set",
      "item": [
        {
          "id": "ef3cb2db-b0fd-4537-91cb-782da1f19105",
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
              "id": "a6dac34f-a555-4b07-93d7-c7c4987370b6"
            }
          ]
        },
        {
          "id": "24709179-f1a2-4fde-81c0-298426513e41",
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
              "id": "346e8ef6-11de-4223-8fef-d29dae9328de"
            }
          ]
        },
        {
          "id": "7dc48c8d-2205-4687-ae0e-c91c61240aad",
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
              "id": "550387a2-32fb-4668-a535-f5f47612c0e7"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Sets",
      "item": [
        {
          "id": "cdc32c94-14fe-4fa6-8d98-3aedc24a32c4",
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
              "id": "1f5888a5-9a7f-4fe7-92b1-004f3bf19e75"
            }
          ]
        },
        {
          "id": "f170f96f-06bc-4ac2-ba4c-bdd6a17a41a6",
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
              "id": "22ec6171-df1e-4c18-a6cb-74a4a3a8026a"
            }
          ]
        },
        {
          "id": "a196092d-b231-4488-ab5e-f88776a5e7f9",
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
              "id": "50c29628-b851-4921-ae38-74abdc062edd"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "0768211d-72a9-4dd2-9c4b-9b06c361b3cb",
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
              "id": "fa0ee01e-0470-4c11-a8eb-748e8c9342be"
            }
          ]
        },
        {
          "id": "ad34851b-fa30-413c-8570-a2d71c8871b2",
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
              "id": "abfffead-28cd-48ca-9f25-9ea3320538aa"
            }
          ]
        },
        {
          "id": "36fe76cc-e9f5-48cb-9f90-382e31932a38",
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
              "id": "aa31ef31-36b1-4374-bec1-3ae1e106cb89"
            }
          ]
        }
      ]
    },
    {
      "name": "Size Constraint Set",
      "item": [
        {
          "id": "a0befabe-9273-4432-91f2-2a8ce7c97772",
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
              "id": "9fdd2c2e-5e40-4afc-b882-f83bec11e1ec"
            }
          ]
        },
        {
          "id": "ee3500fd-347f-44fd-b2e8-15ff9b5b0294",
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
              "id": "4dce7490-2b3e-4228-86bb-65536621e305"
            }
          ]
        },
        {
          "id": "b0efa4e4-afcd-4519-acd5-f9c78f0ab95e",
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
              "id": "e1c94514-763c-4c68-88cb-2243430c4534"
            }
          ]
        }
      ]
    },
    {
      "name": "SQL Injection Match Set",
      "item": [
        {
          "id": "bac2fd49-b8b1-4796-90e5-eefc8c38a29b",
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
              "id": "d22e9ea5-be6c-4966-bcdf-a9dbedbc4da9"
            }
          ]
        },
        {
          "id": "a74e5456-0afb-427f-8bc9-4bd151d0c04e",
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
              "id": "7afedea1-d409-4b8d-91b0-d4ffa7fb0fd7"
            }
          ]
        }
      ]
    },
    {
      "name": "XSS Match Set",
      "item": [
        {
          "id": "f1f8734e-2a33-4a8b-a12b-252aca2fb1fc",
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
              "id": "0a4ae220-33bf-4b83-8bfd-b64a3d284424"
            }
          ]
        },
        {
          "id": "7c09fc7c-ebf3-4ca3-8287-f35d2213ab8c",
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
              "id": "a8437f05-6b5e-4380-91d0-0f0f9b83681d"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Token",
      "item": [
        {
          "id": "d57cf963-456f-41a4-aa2c-934282b35b61",
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
              "id": "37b0e42f-b0ee-4edf-b076-596fa94b5c87"
            }
          ]
        },
        {
          "id": "ec44a10b-8953-4757-8735-3b42aece4070",
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
              "id": "4536be4e-732a-4b61-a6fb-ced77480a2d5"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "0c27cd18-28ce-4d28-85fd-e71beaaf06ae",
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
              "id": "c86c4eda-94d8-437c-9790-020bbfb9c0be"
            }
          ]
        }
      ]
    }
  ]
}