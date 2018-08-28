{
  "info": {
    "name": "AWS Direct Connect API Describe Interconnect Loa",
    "_postman_id": "ba2922c4-997c-4d40-872c-2ac7eeeb7579",
    "description": "Returns the LOA-CFA for an Interconnect.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Connections",
      "item": [
        {
          "id": "b8d79cf1-8222-4b56-b24f-d2c9e6f6b659",
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
              "id": "45e5ebb4-c34b-46a4-ba14-b8fbb962f830"
            }
          ]
        },
        {
          "id": "0ff3fae4-e456-4dfa-8c85-9af31919e68e",
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
              "id": "03108c7f-f310-4cad-a81e-719f7706b855"
            }
          ]
        },
        {
          "id": "856bd60d-14fc-453a-b944-9051f863e5af",
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
              "id": "6daf3d1f-c20c-4d5e-bd10-e868720d541a"
            }
          ]
        },
        {
          "id": "a010d2a1-1083-4dd3-885f-69e6295592e9",
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
              "id": "2eee66dc-cc5e-481b-bceb-853622ca4439"
            }
          ]
        },
        {
          "id": "7f69c7c8-3776-4c44-81ac-7386f5bdf2b5",
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
              "id": "fbc1bb27-c7f4-4401-a531-ddac53b6b6bf"
            }
          ]
        },
        {
          "id": "42d91dd9-4675-4004-a980-cf87417616ee",
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
              "id": "f7627351-cabe-41ec-ae80-47558f58c076"
            }
          ]
        },
        {
          "id": "50e02cf5-6c20-4a08-bb24-d6aa007c1835",
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
              "id": "7ea6bdf0-dbfd-4c5a-b29e-798f6f506b27"
            }
          ]
        }
      ]
    },
    {
      "name": "Private Virtual Interfaces",
      "item": [
        {
          "id": "83dc4672-6eed-412c-a428-b81d532c89bf",
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
              "id": "2e3995b4-9f41-4568-8706-f40ff0069d08"
            }
          ]
        },
        {
          "id": "af36f0d2-4b73-4bb2-922e-637ecf83a2da",
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
              "id": "38afb29a-e39a-4e97-a762-6247c68b151b"
            }
          ]
        },
        {
          "id": "d960023e-782a-4d85-bc96-25e6b31ec110",
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
              "id": "d6a5ed1f-78ca-416f-b05e-67c18792a801"
            }
          ]
        },
        {
          "id": "42881db5-eedf-462a-8ba5-a029c82207ec",
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
              "id": "10c2d661-ef15-4838-ab83-fb16d8588472"
            }
          ]
        },
        {
          "id": "fe634f6d-1060-4a37-bcd1-48b3c41ae78e",
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
              "id": "397ed982-1cfc-4044-9931-39acb6fc693a"
            }
          ]
        },
        {
          "id": "20e6e41e-c7fd-4c5e-ad07-8af2a37fe87c",
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
              "id": "313f3cad-bbe6-418a-8626-51319718dfae"
            }
          ]
        }
      ]
    },
    {
      "name": "BGP Peer",
      "item": [
        {
          "id": "4103e99f-7e81-495b-928c-886f23f55d32",
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
              "id": "371b3eec-32e2-4614-863e-75aa706f7b37"
            }
          ]
        },
        {
          "id": "37f891fd-eca6-4972-bb98-b12d21992587",
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
              "id": "249c88c4-c0c5-462b-af1c-92955767669f"
            }
          ]
        }
      ]
    },
    {
      "name": "Interconnects",
      "item": [
        {
          "id": "50b22107-7a5a-47b8-9c3d-98bf6fd3d935",
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
              "id": "93fb9f2a-c37f-434f-99aa-4fadca1fc29a"
            }
          ]
        },
        {
          "id": "62776bdb-4dd4-4fde-a79f-2cdb585875fb",
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
              "id": "e29319c2-3f96-4ecc-8812-8f36035522b9"
            }
          ]
        },
        {
          "id": "feff6655-ba7f-45cc-b7cb-6b5c2f33ad04",
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
              "id": "580ea149-3699-413c-85d7-3f039f44d464"
            }
          ]
        }
      ]
    },
    {
      "name": "Virtual Interfaces",
      "item": [
        {
          "id": "08a8b83d-6afb-4ced-a6f8-2e4fefb0f083",
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
              "id": "74573efc-d84a-45fd-bdea-1829af0650a5"
            }
          ]
        }
      ]
    }
  ]
}