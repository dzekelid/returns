{
  "info": {
    "name": "Amazon Lightsale API Is Vpc Peered",
    "_postman_id": "def570bf-3775-4601-beb8-7231d5896efa",
    "description": "Returns a Boolean value indicating whether your Lightsail VPC is peered.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "9e16ed1b-8900-4cf3-a1e9-76924d773740",
          "name": "allocateStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=AllocateStaticIp?staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allocates a static IP address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d19829ec-3120-463f-97a0-0f7060696981"
            }
          ]
        },
        {
          "id": "1b23a516-fd91-4635-a9ad-112f61eaab86",
          "name": "attachStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=AttachStaticIp?instanceName=instanceName&staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches a static IP address to a specific Amazon Lightsail instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2695d75-aaf4-47b9-8b6f-9eeae474455e"
            }
          ]
        },
        {
          "id": "5c777c38-9b11-4e35-b2a5-311aa90ea270",
          "name": "detachStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=DetachStaticIp?staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches a static IP from the Amazon Lightsail instance to which it is\n      attached."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f99f96ea-b41e-4a28-a4e9-9dcf5e81b56a"
            }
          ]
        },
        {
          "id": "9791945d-04c9-4617-90f5-67b8271a0360",
          "name": "getStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=GetStaticIp?staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific static IP."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5c8981f-8384-40fd-9e42-a0d831d9347a"
            }
          ]
        },
        {
          "id": "67d77a8d-b258-4024-a4ca-c7018425d4cb",
          "name": "getStaticIps",
          "request": {
            "url": "http://example.com/api/?Action=GetStaticIps?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all static IPs in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd70a6cb-d787-4642-9b4d-5052c1921998"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "69f5a209-5134-45a2-b45f-f7f50ab9f5dc",
          "name": "closeInstancePublicPorts",
          "request": {
            "url": "http://example.com/api/?Action=CloseInstancePublicPorts?instanceName=instanceName&portInfo=portInfo",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Closes the public ports on a specific Amazon Lightsail instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ceb0d9e3-facb-456b-a269-d8c619e40b6c"
            }
          ]
        },
        {
          "id": "7c1cb99a-481f-4d6a-8faa-a6b94406bdf7",
          "name": "createInstances",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstances?availabilityZone=availabilityZone&blueprintId=blueprintId&bundleId=bundleId&customImageName=customImageName&instanceNames=instanceNames&keyPairName=keyPairName&userData=userData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates one or more Amazon Lightsail virtual private servers, or\n        instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6188323c-0dda-4fa3-b229-03e8a2d20387"
            }
          ]
        },
        {
          "id": "672dd753-a5aa-4255-b323-7bc0c947ec51",
          "name": "createInstancesFromSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstancesFromSnapshot?availabilityZone=availabilityZone&bundleId=bundleId&instanceNames=instanceNames&instanceSnapshotName=instanceSnapshotName&keyPairName=keyPairName&userData=userData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uses a specific snapshot as a blueprint for creating one or more new instances that are\n      based on that identical configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dead534-1c8c-4da4-aaa6-4ba2236728ac"
            }
          ]
        },
        {
          "id": "8685b594-6579-4b1f-9160-d630ff6c8bb3",
          "name": "createInstanceSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstanceSnapshot?instanceName=instanceName&instanceSnapshotName=instanceSnapshotName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a specific virtual private server, or\n        instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc387895-93c1-47ac-9a10-71aa1cac599a"
            }
          ]
        },
        {
          "id": "21bc046e-8c9b-47cc-ad26-7981d78c42c2",
          "name": "deleteInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInstance?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific Amazon Lightsail virtual private server, or\n        instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e208fab-7596-4a8e-90bb-8e873c4c9138"
            }
          ]
        },
        {
          "id": "311fcbef-27c7-47fd-8a06-41811d9f1845",
          "name": "deleteInstanceSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInstanceSnapshot?instanceSnapshotName=instanceSnapshotName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific snapshot of a virtual private server (or\n        instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82a7fdd7-a9d4-45ac-b27b-4b09338f427f"
            }
          ]
        },
        {
          "id": "47e3dc07-f084-4b3b-8854-8619876454a1",
          "name": "getBlueprints",
          "request": {
            "url": "http://example.com/api/?Action=GetBlueprints?includeInactive=includeInactive&pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of available instance images, or blueprints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da17f07d-6a90-411d-b127-a85ba3155cd8"
            }
          ]
        },
        {
          "id": "b9a7aa1b-fa52-4a29-aab6-8c31cd57b2aa",
          "name": "getInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetInstance?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific Amazon Lightsail instance, which is a virtual\n      private server."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "368b555b-6852-4c9e-b78c-ab25edd089b6"
            }
          ]
        },
        {
          "id": "9c2d2990-ca44-43cf-9cff-fb17263c2af8",
          "name": "getInstanceAccessDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceAccessDetails?instanceName=instanceName&protocol=protocol",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns temporary SSH keys you can use to connect to a specific virtual private server,\n      or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09b43bc9-c036-4191-8f92-f8098ff05046"
            }
          ]
        },
        {
          "id": "9fb54e9d-3006-4813-aca6-e1e2ba147dd3",
          "name": "getInstanceMetricData",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceMetricData?endTime=endTime&instanceName=instanceName&metricName=metricName&period=period&startTime=startTime&statistics=statistics&unit=unit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the data points for the specified Amazon Lightsail instance metric, given an\n      instance name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c36d0fe-9544-4919-a9f4-b8f894872074"
            }
          ]
        },
        {
          "id": "55451d06-d06f-42b8-86df-4c845114d353",
          "name": "getInstancePortStates",
          "request": {
            "url": "http://example.com/api/?Action=GetInstancePortStates?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the port states for a specific virtual private server, or\n        instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "558ce952-cfaf-4e87-bdf8-b8818f7ac7ea"
            }
          ]
        },
        {
          "id": "d3368f35-5786-49e9-9e81-d929d0e8a0c2",
          "name": "getInstances",
          "request": {
            "url": "http://example.com/api/?Action=GetInstances?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all Amazon Lightsail virtual private servers, or\n        instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "869cebce-2db8-43d6-9d9c-3d4b260d0e5c"
            }
          ]
        },
        {
          "id": "57234f4f-ee44-4d28-938d-07532ec34288",
          "name": "getInstanceSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceSnapshot?instanceSnapshotName=instanceSnapshotName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific instance snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8be845b7-4e74-40d9-a77b-5522bf36865f"
            }
          ]
        },
        {
          "id": "a8bbb6b0-ebf5-40ae-beff-d7356ab9d80d",
          "name": "getInstanceSnapshots",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceSnapshots?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all instance snapshots for the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc710e0b-0096-4417-9656-13253ae702cb"
            }
          ]
        },
        {
          "id": "59468aa3-bda6-4528-975d-b6740a8dd06c",
          "name": "getInstanceState",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceState?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the state of a specific instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32ea0e4a-8a6b-415f-8927-2cb2810d9461"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "180e3c12-e199-43bd-8971-ca8943349ff5",
          "name": "createDomain",
          "request": {
            "url": "http://example.com/api/?Action=CreateDomain?domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a domain resource for the specified domain (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58574148-89bb-4d82-9393-4c0479c7460e"
            }
          ]
        },
        {
          "id": "c90192ea-b0d7-4dbd-8f0e-27daef454cd8",
          "name": "createDomainEntry",
          "request": {
            "url": "http://example.com/api/?Action=CreateDomainEntry?domainEntry=domainEntry&domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates one of the following entry records associated with the domain: A record, CNAME\n      record, TXT record, or MX record."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9140816b-f42a-45d6-ae35-7ceb518e0855"
            }
          ]
        },
        {
          "id": "f28a8aef-e031-49eb-bf94-c72e9c490bf8",
          "name": "deleteDomain",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDomain?domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified domain recordset and all of its domain records."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bccaef69-95a3-4d6c-ae2a-fa378f975931"
            }
          ]
        },
        {
          "id": "8f4bc363-454b-47cb-9e9c-81711b0e42e4",
          "name": "deleteDomainEntry",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDomainEntry?domainEntry=domainEntry&domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific domain entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "114acc54-d55c-4255-b7b2-eb2950caf233"
            }
          ]
        },
        {
          "id": "00a00293-b7f9-4d3b-8148-848429e65c62",
          "name": "getDomain",
          "request": {
            "url": "http://example.com/api/?Action=GetDomain?domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific domain recordset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "602e2b4a-1f8d-4403-a34f-dd27d2039747"
            }
          ]
        },
        {
          "id": "277cd440-31f3-43f7-9d4b-02cce563d89a",
          "name": "getDomains",
          "request": {
            "url": "http://example.com/api/?Action=GetDomains?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all domains in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b49a5ce7-2af1-44f7-94ac-8504b5f0589e"
            }
          ]
        }
      ]
    },
    {
      "name": "Key Pairs",
      "item": [
        {
          "id": "48e6a4bb-a241-4dcd-8c30-ffd1ad9a4b6e",
          "name": "createKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=CreateKeyPair?keyPairName=keyPairName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates sn SSH key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23c03dd2-9fcf-4b8e-a03b-9a3ed5176434"
            }
          ]
        },
        {
          "id": "30bdb079-b8d6-4c95-9734-6deded52c0e5",
          "name": "deleteKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=DeleteKeyPair?keyPairName=keyPairName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific SSH key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc4844e0-2aed-48ff-ac35-504be7ddd9ff"
            }
          ]
        },
        {
          "id": "b7fceef8-8d5f-4a1e-9a8c-518c8ad86fcc",
          "name": "downloadDefaultKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=DownloadDefaultKeyPair?privateKeyBase64=privateKeyBase64&publicKeyBase64=publicKeyBase64",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Downloads the default SSH key pair from the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac31d915-d1fa-4ee2-8fbe-e779c761f37d"
            }
          ]
        },
        {
          "id": "90893382-0cba-4f6f-b60a-51a374cf03d1",
          "name": "getKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=GetKeyPair?keyPairName=keyPairName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abde9ba7-d657-49a3-b0e1-043467a4a01d"
            }
          ]
        },
        {
          "id": "4ae4c0b5-ba43-449a-9106-fb665b5aab34",
          "name": "getKeyPairs",
          "request": {
            "url": "http://example.com/api/?Action=GetKeyPairs?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all key pairs in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef4d599d-ae80-4802-82b8-40ed9870b70e"
            }
          ]
        },
        {
          "id": "6615c14c-c329-42b2-8364-cd631c7e6303",
          "name": "importKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=ImportKeyPair?keyPairName=keyPairName&publicKeyBase64=publicKeyBase64",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Imports a public SSH key from a specific key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "272e73f9-4502-4cc6-b966-f3de5e8b6726"
            }
          ]
        }
      ]
    },
    {
      "name": "Names",
      "item": [
        {
          "id": "223e8549-dfba-439e-bf7c-08c6b628f3b2",
          "name": "getActiveNames",
          "request": {
            "url": "http://example.com/api/?Action=GetActiveNames?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the names of all active (not deleted) resources."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2eb0408-3390-45f5-91f0-858c59ee9b3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Bundles",
      "item": [
        {
          "id": "1d0ea2f2-45f9-4f96-b7be-435a573f27bb",
          "name": "getBundles",
          "request": {
            "url": "http://example.com/api/?Action=GetBundles?includeInactive=includeInactive&pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of bundles that are available for purchase."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a498c91-cc54-44f8-b4aa-6f3126ccd7fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Operations",
      "item": [
        {
          "id": "22888005-90e8-4a7a-9c10-e2fd1aed00b3",
          "name": "getOperation",
          "request": {
            "url": "http://example.com/api/?Action=GetOperation?operationId=operationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific operation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d631bda8-6731-4b50-b03e-8df6017b15b7"
            }
          ]
        },
        {
          "id": "b7347574-500d-4a49-95d7-56070b4642a2",
          "name": "getOperations",
          "request": {
            "url": "http://example.com/api/?Action=GetOperations?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0ca0896-0af6-4646-bf2b-d63db310fca9"
            }
          ]
        },
        {
          "id": "ecb0a87e-bbaf-4a91-9a06-97cc5e58ac5b",
          "name": "getOperationsForResource",
          "request": {
            "url": "http://example.com/api/?Action=GetOperationsForResource?pageToken=pageToken&resourceName=resourceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets operations for a specific resource (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "357aa6c4-8366-44f6-a6a8-fbe2bbbc3b1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "822a12fd-eeec-48f8-a30d-ab1dd5b61ff5",
          "name": "getRegions",
          "request": {
            "url": "http://example.com/api/?Action=GetRegions?includeAvailabilityZones=includeAvailabilityZones",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all valid regions for Amazon Lightsail."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e581755b-6400-4ae5-9ffe-c9a2ab8f33a7"
            }
          ]
        }
      ]
    },
    {
      "name": "VPC",
      "item": [
        {
          "id": "40766ba1-cfb1-4905-bafd-ec0ba6fd1363",
          "name": "isVpcPeered",
          "request": {
            "url": "http://example.com/api/?Action=IsVpcPeered?isPeered=isPeered",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a Boolean value indicating whether your Lightsail VPC is peered."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16f52db9-ea25-4252-ba77-c5fefc6b16d1"
            }
          ]
        }
      ]
    }
  ]
}