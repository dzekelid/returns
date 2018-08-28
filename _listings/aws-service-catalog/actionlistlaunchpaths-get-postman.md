{
  "info": {
    "name": "AWS Service Catalog API List Launch Paths",
    "_postman_id": "c702de07-48f7-40f6-9e9c-0cb2b31a51ec",
    "description": "Returns a paginated list of all paths to a specified product.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Portfolios",
      "item": [
        {
          "id": "a28b5f7d-85db-4edf-9166-5b5ce24edd2a",
          "name": "acceptPortfolioShare",
          "request": {
            "url": "http://example.com/api/?Action=AcceptPortfolioShare?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts an offer to share a portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5eb13925-7d20-4e1e-bc2e-a0a565a03222"
            }
          ]
        },
        {
          "id": "dd7ae751-aeec-4892-a8b3-a09f9b80b501",
          "name": "associatePrincipalWithPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=AssociatePrincipalWithPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&PrincipalARN=PrincipalARN&PrincipalType=PrincipalType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified principal ARN with the specified portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3a450b4-0170-4ec1-bf89-5f37512c7d0d"
            }
          ]
        },
        {
          "id": "4b5d9bc4-2a49-4f51-9bc5-e133487f893e",
          "name": "associateProductWithPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=AssociateProductWithPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&ProductId=ProductId&SourcePortfolioId=SourcePortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates a product with a portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b9355bd-2287-44bf-9063-64a800410f59"
            }
          ]
        },
        {
          "id": "95f76e82-ab3b-43c8-8770-4afccbe43e03",
          "name": "createPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=CreatePortfolio?AcceptLanguage=AcceptLanguage&Description=Description&DisplayName=DisplayName&IdempotencyToken=IdempotencyToken&ProviderName=ProviderName&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fc41460-6d34-4b7d-a7c2-bc2dcb398854"
            }
          ]
        },
        {
          "id": "fe16e562-401c-4b6c-8cf3-988196b77e79",
          "name": "createPortfolioShare",
          "request": {
            "url": "http://example.com/api/?Action=CreatePortfolioShare?AcceptLanguage=AcceptLanguage&AccountId=AccountId&PortfolioId=PortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new portfolio share."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe73faf7-44ee-4fb1-a024-3ba193e69d9c"
            }
          ]
        },
        {
          "id": "a3400293-53a3-4523-9528-05bb59c545da",
          "name": "deletePortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DeletePortfolio?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c99d3cef-fa42-40b5-bcc7-d88ab1110519"
            }
          ]
        },
        {
          "id": "96e661e1-d03d-42c2-ae38-f84c7a5fd224",
          "name": "deletePortfolioShare",
          "request": {
            "url": "http://example.com/api/?Action=DeletePortfolioShare?AcceptLanguage=AcceptLanguage&AccountId=AccountId&PortfolioId=PortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified portfolio share."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8899e81-6f45-468b-85d2-45dd343cff26"
            }
          ]
        },
        {
          "id": "27173164-d70f-42e5-b974-c75471d17e3c",
          "name": "describePortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DescribePortfolio?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves detailed information and any tags associated with the specified\n         portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "269e08bf-951f-44f7-a660-c45ae09c412b"
            }
          ]
        },
        {
          "id": "b8fed80b-7242-4036-a858-56e047926de9",
          "name": "disassociatePrincipalFromPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DisassociatePrincipalFromPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&PrincipalARN=PrincipalARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates a previously associated principal ARN from a specified\n         portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "684a5d03-89c0-4612-a566-51711a769c22"
            }
          ]
        },
        {
          "id": "429915a2-26ea-4988-9c1f-8314dd06b021",
          "name": "disassociateProductFromPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateProductFromPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&ProductId=ProductId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified product from the specified portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6891a242-40b7-4e75-99f7-81a073a40bea"
            }
          ]
        },
        {
          "id": "728486d0-47b2-4dc9-8cd1-ef96ef676d31",
          "name": "listAcceptedPortfolioShares",
          "request": {
            "url": "http://example.com/api/?Action=ListAcceptedPortfolioShares?AcceptLanguage=AcceptLanguage&PageSize=PageSize&PageToken=PageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists details of all portfolios for which sharing was accepted by this\n         account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "711473f6-a56a-47c9-944d-501c431a69ee"
            }
          ]
        },
        {
          "id": "e7badfd7-9bd6-4aa2-b9c3-4d7e9539e1a8",
          "name": "listConstraintsForPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=ListConstraintsForPortfolio?AcceptLanguage=AcceptLanguage&PageSize=PageSize&PageToken=PageToken&PortfolioId=PortfolioId&ProductId=ProductId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves detailed constraint information for the specified portfolio and\n         product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb220dd4-ed96-405d-ac09-c1ab3f208ecf"
            }
          ]
        }
      ]
    },
    {
      "name": "Constraints",
      "item": [
        {
          "id": "0936271c-5a92-4cae-9ddb-3ea8a11677c5",
          "name": "createConstraint",
          "request": {
            "url": "http://example.com/api/?Action=CreateConstraint?AcceptLanguage=AcceptLanguage&Description=Description&IdempotencyToken=IdempotencyToken&Parameters=Parameters&PortfolioId=PortfolioId&ProductId=ProductId&Type=Type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new constraint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a37da1b-af9f-4e46-9f3e-7cd2041518dc"
            }
          ]
        },
        {
          "id": "95a268d9-2b82-4da0-9f43-e43b5a4d37d5",
          "name": "deleteConstraint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConstraint?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified constraint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4650904e-be05-431c-a74c-8e2522a719ea"
            }
          ]
        },
        {
          "id": "6ba2240a-3fb4-4fbb-8c0d-b5e74424171f",
          "name": "describeConstraint",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConstraint?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves detailed information for a specified constraint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9c20d95-a53a-4ef1-b724-3e5774858ea4"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "fb961a6a-eb96-4049-9dba-cea150c0c108",
          "name": "createProduct",
          "request": {
            "url": "http://example.com/api/?Action=CreateProduct?AcceptLanguage=AcceptLanguage&Description=Description&Distributor=Distributor&IdempotencyToken=IdempotencyToken&Name=Name&Owner=Owner&ProductType=ProductType&ProvisioningArtifactParameters=ProvisioningArtifactParameters&SupportDescription=SupportDescription&SupportEmail=SupportEmail&SupportUrl=SupportUrl&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2a9100b-478f-4f70-8bfb-672e04c3d662"
            }
          ]
        },
        {
          "id": "3fe22e02-f7b7-43b2-bd3d-95acc2d101ce",
          "name": "deleteProduct",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProduct?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "695cb5db-e974-4de2-b3e8-e91f56bfb5eb"
            }
          ]
        },
        {
          "id": "c99bc63d-4f30-476b-9bcd-306f768a69fa",
          "name": "describeProduct",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProduct?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8e218da-c8fe-48e0-bfe9-2267cebe2028"
            }
          ]
        },
        {
          "id": "47bbe3fb-7de7-4ee3-9d5f-4cd533e17fad",
          "name": "describeProductAsAdmin",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProductAsAdmin?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a specified product, run with administrator\n         access."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebffcd74-7dd5-4833-8af4-c31dd60edf2d"
            }
          ]
        },
        {
          "id": "21e6ceb9-e479-4faf-82b4-73abebfaff7a",
          "name": "describeProductView",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProductView?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40f1bef7-dccb-4893-ad94-203c7f8f5782"
            }
          ]
        }
      ]
    },
    {
      "name": "Provisioning Artifacts",
      "item": [
        {
          "id": "32aefd67-7c05-4434-81cd-901f13a77459",
          "name": "createProvisioningArtifact",
          "request": {
            "url": "http://example.com/api/?Action=CreateProvisioningArtifact?AcceptLanguage=AcceptLanguage&IdempotencyToken=IdempotencyToken&Parameters=Parameters&ProductId=ProductId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new provisioning artifact for the specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5f40299-6436-4f61-a9bb-13534a186b6e"
            }
          ]
        },
        {
          "id": "c21aec25-30da-43b3-871f-e9a33a144780",
          "name": "deleteProvisioningArtifact",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProvisioningArtifact?AcceptLanguage=AcceptLanguage&ProductId=ProductId&ProvisioningArtifactId=ProvisioningArtifactId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified provisioning artifact."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27d6df5e-0cde-4606-bdac-e234051e4004"
            }
          ]
        },
        {
          "id": "fa9cf293-a5f7-4902-8087-45dfa9da8f7f",
          "name": "describeProvisioningArtifact",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProvisioningArtifact?AcceptLanguage=AcceptLanguage&ProductId=ProductId&ProvisioningArtifactId=ProvisioningArtifactId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves detailed information about the specified provisioning artifact."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ca3c956-67c2-49c1-a324-6f397b360284"
            }
          ]
        }
      ]
    },
    {
      "name": "Provisioning Parameters",
      "item": [
        {
          "id": "6933f9fe-9f65-47bb-97d8-711d7faac172",
          "name": "describeProvisioningParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProvisioningParameters?AcceptLanguage=AcceptLanguage&PathId=PathId&ProductId=ProductId&ProvisioningArtifactId=ProvisioningArtifactId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about parameters required to provision a specified product in a\n         specified manner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf1859b5-232d-42fa-a481-ed4762bd5d08"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "a50e98c1-c21c-4d28-b540-d7508b1a68d6",
          "name": "describeRecord",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRecord?AcceptLanguage=AcceptLanguage&Id=Id&PageSize=PageSize&PageToken=PageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a paginated list of the full details of a specific request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4c926ee-12a1-4911-90f7-d9f136f3f2f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Launch Paths",
      "item": [
        {
          "id": "a647a7e0-db1b-40b6-a47b-91930d856f9c",
          "name": "listLaunchPaths",
          "request": {
            "url": "http://example.com/api/?Action=ListLaunchPaths?AcceptLanguage=AcceptLanguage&PageSize=PageSize&PageToken=PageToken&ProductId=ProductId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated list of all paths to a specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e298c4f3-0924-40d0-952b-2cfb03d7bad9"
            }
          ]
        }
      ]
    }
  ]
}