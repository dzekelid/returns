{
  "info": {
    "name": "AWS Direct Connect API Describe Interconnects",
    "_postman_id": "5e110863-c4c5-4078-b575-92b16ffe04e1",
    "description": "Returns a list of interconnects owned by the AWS account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Connections",
      "item": [
        {
          "id": "367f55d8-5b48-48c3-95ec-a12023bc5292",
          "name": "allocateConnectionOnInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=AllocateConnectionOnInterconnect?bandwidth=bandwidth&connectionName=connectionName&interconnectId=interconnectId&ownerAccount=ownerAccount&vlan=vlan",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a hosted connection on an interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d762f91a-c786-42a7-959d-bd861bf070c2"
            }
          ]
        },
        {
          "id": "95ab77ce-294c-4e16-882c-b7a9efd74db4",
          "name": "confirmConnection",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmConnection?connectionId=connectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirm the creation of a hosted connection on an interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8af87d2f-43e2-480e-be11-16a9c673170e"
            }
          ]
        },
        {
          "id": "b4b825cf-34ce-4fe9-b77d-0529b4e6f619",
          "name": "createConnection",
          "request": {
            "url": "http://example.com/api/?Action=CreateConnection?bandwidth=bandwidth&connectionName=connectionName&location=location",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new connection between the customer network and a specific AWS Direct Connect location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c3c7435-2dc6-4e53-9895-359fb5547144"
            }
          ]
        },
        {
          "id": "95091787-e384-419d-abd8-9b8959df7bae",
          "name": "deleteConnection",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConnection?connectionId=connectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the connection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dab2bc3e-4cef-422b-b460-288446984af3"
            }
          ]
        },
        {
          "id": "3cc15c24-de6d-4b46-84e8-8f373fda9cbe",
          "name": "describeConnectionLoa",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConnectionLoa?connectionId=connectionId&loaContentType=loaContentType&providerName=providerName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the LOA-CFA for a Connection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb20a235-8045-43b5-b3ea-86af4950e365"
            }
          ]
        },
        {
          "id": "06f1fe9e-51c2-46fe-ab9f-099ef1f1d8fa",
          "name": "describeConnections",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConnections?connectionId=connectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Displays all connections in this region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4319a410-a8cc-472e-aa3f-f57619fe22f5"
            }
          ]
        },
        {
          "id": "441b3792-46b4-49f3-9894-e6560f049b40",
          "name": "describeConnectionsOnInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConnectionsOnInterconnect?interconnectId=interconnectId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of connections that have been provisioned on the given interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0c22aee-c958-4f6d-a4cd-afb1857999cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Private Virtual Interfaces",
      "item": [
        {
          "id": "a49b3b7e-3533-48a2-a0f3-3d5c9471dc3c",
          "name": "allocatePrivateVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=AllocatePrivateVirtualInterface?connectionId=connectionId&newPrivateVirtualInterfaceAllocation=newPrivateVirtualInterfaceAllocation&ownerAccount=ownerAccount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provisions a private virtual interface to be owned by a different customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19f6f4b4-e98b-4a73-9432-b915f2bbc1a2"
            }
          ]
        },
        {
          "id": "198f3dfb-7718-4d0e-969e-55add0e6ad38",
          "name": "allocatePublicVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=AllocatePublicVirtualInterface?connectionId=connectionId&newPublicVirtualInterfaceAllocation=newPublicVirtualInterfaceAllocation&ownerAccount=ownerAccount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provisions a public virtual interface to be owned by a different customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0b4cab9-896e-4527-9d26-031a9c43308b"
            }
          ]
        },
        {
          "id": "ca61f3d5-338d-4a6f-b859-efc84e5544e7",
          "name": "confirmPrivateVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmPrivateVirtualInterface?virtualGatewayId=virtualGatewayId&virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accept ownership of a private virtual interface created by another customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c77d102-3070-45de-9766-1298dd12ccc6"
            }
          ]
        },
        {
          "id": "192e42f1-463d-462f-a4bd-125dd6881e66",
          "name": "confirmPublicVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmPublicVirtualInterface?virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accept ownership of a public virtual interface created by another customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6be9a53d-6481-4313-907f-8041f9d89483"
            }
          ]
        },
        {
          "id": "e280f2d1-ded9-43c4-b270-98de961d612c",
          "name": "createPrivateVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=CreatePrivateVirtualInterface?connectionId=connectionId&newPrivateVirtualInterface=newPrivateVirtualInterface",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new private virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd523d80-cfb8-4ef8-98fd-184ea6ecb3cf"
            }
          ]
        },
        {
          "id": "6e10bebf-80ef-4472-853e-f2e89751ee13",
          "name": "createPublicVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=CreatePublicVirtualInterface?connectionId=connectionId&newPublicVirtualInterface=newPublicVirtualInterface",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new public virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78c49e19-5cdd-46f5-bcfa-a306356025ab"
            }
          ]
        }
      ]
    },
    {
      "name": "BGP Peer",
      "item": [
        {
          "id": "27545709-1626-4550-91ef-e053e7f21b52",
          "name": "createBGPPeer",
          "request": {
            "url": "http://example.com/api/?Action=CreateBGPPeer?newBGPPeer=newBGPPeer&virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new BGP peer on a specified virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1023ff78-dc00-466b-b423-bf09d290d4bb"
            }
          ]
        },
        {
          "id": "4dc96d78-7a16-4892-b07b-4dc96dba8a87",
          "name": "deleteBGPPeer",
          "request": {
            "url": "http://example.com/api/?Action=DeleteBGPPeer?asn=asn&customerAddress=customerAddress&virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a BGP peer on the specified virtual interface that matches the specified customer address and ASN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4babb897-8b55-4ca0-9ce7-fcd8c606df54"
            }
          ]
        }
      ]
    },
    {
      "name": "Interconnects",
      "item": [
        {
          "id": "c6f776f4-4b58-4612-a2e9-597ccae13462",
          "name": "createInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=CreateInterconnect?bandwidth=bandwidth&interconnectName=interconnectName&location=location",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new interconnect between a AWS Direct Connect partner's network and a specific AWS Direct Connect location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f76074b0-33c4-417b-888a-303452e490a0"
            }
          ]
        },
        {
          "id": "50c47734-512d-4bf9-b881-8595cc1ed183",
          "name": "deleteInterconnect",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInterconnect?interconnectId=interconnectId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d25a5c26-e594-4a65-9911-27c9840fc549"
            }
          ]
        },
        {
          "id": "c5791ffc-67ad-4e36-a18b-e6ae5e2a1cd0",
          "name": "describeInterconnectLoa",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInterconnectLoa?interconnectId=interconnectId&loaContentType=loaContentType&providerName=providerName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the LOA-CFA for an Interconnect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66fb842c-bba8-4b21-8db7-10f393bfb97f"
            }
          ]
        },
        {
          "id": "413696b5-ea61-4888-9eb6-05cb8803c78f",
          "name": "describeInterconnects",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInterconnects?interconnectId=interconnectId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of interconnects owned by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae5ea2b7-04e7-4452-b0c9-9e3650fd5f52"
            }
          ]
        }
      ]
    },
    {
      "name": "Virtual Interfaces",
      "item": [
        {
          "id": "9dcf4d50-f12a-4da2-ad95-1d49779d60af",
          "name": "deleteVirtualInterface",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVirtualInterface?virtualInterfaceId=virtualInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a virtual interface."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa1a1ea0-342f-425a-a013-0cfaee63e016"
            }
          ]
        }
      ]
    }
  ]
}