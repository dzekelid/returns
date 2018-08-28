{
  "info": {
    "name": "AWS Storage Gateway Service API Describe Bandwidth Rate Limit",
    "_postman_id": "b821a153-ee5f-4a31-ae7b-4d55af838f6d",
    "description": "Returns the bandwidth rate limits of a gateway.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "2937c27f-4b2e-4902-8daf-1c5673b577b4",
          "name": "activateGateway",
          "request": {
            "url": "http://example.com/api/?Action=ActivateGateway?ActivationKey=ActivationKey&GatewayName=GatewayName&GatewayRegion=GatewayRegion&GatewayTimezone=GatewayTimezone&GatewayType=GatewayType&MediumChangerType=MediumChangerType&TapeDriveType=TapeDriveType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activates the gateway you previously deployed on your host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca5391ef-dfc6-4ef0-b712-bca699c5424a"
            }
          ]
        },
        {
          "id": "74a04c0f-fe95-4d19-bb99-42324a7a399b",
          "name": "deleteGateway",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGateway?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f966b574-3b4a-4c1f-b8b8-997f24200c7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "ab9656b1-87fa-48f5-8e4a-904c21e7d637",
          "name": "addCache",
          "request": {
            "url": "http://example.com/api/?Action=AddCache?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as cache for a cached-volume gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d51542d-4ad7-41f6-887e-f8794ee9cb7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "cd1d2839-3b79-4b87-b363-7b5b0a5d8951",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceARN=ResourceARN&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds one or more tags to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "373dd809-fb85-4c99-b87d-5bcc508922be"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "b52a4dde-8a0f-4bd4-bc6f-099a8671aea8",
          "name": "addUploadBuffer",
          "request": {
            "url": "http://example.com/api/?Action=AddUploadBuffer?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as upload buffer for a specified gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ae15eea-aea1-4adc-8905-35c887e7964a"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "d5c6d801-4e26-4176-8e44-294ddd601e5d",
          "name": "addWorkingStorage",
          "request": {
            "url": "http://example.com/api/?Action=AddWorkingStorage?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as working storage for a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "127c2cad-b01a-4e55-bfb0-2a4492b1b1b7"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "d665c97b-a902-4f9f-81e9-efafd2987409",
          "name": "cancelArchival",
          "request": {
            "url": "http://example.com/api/?Action=CancelArchival?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels archiving of a virtual tape to the virtual tape shelf (VTS) after the\n         archiving process is initiated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "095ed426-d2ab-48df-a716-9face81f5b75"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "e6643352-edc0-4927-961c-bf90f70e18dc",
          "name": "cancelRetrieval",
          "request": {
            "url": "http://example.com/api/?Action=CancelRetrieval?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels retrieval of a virtual tape from the virtual tape shelf (VTS) to a gateway\n         after the retrieval process is initiated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c2e2de9-1e9d-4b9f-80b9-cb1642a00a47"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "77c99e02-757a-4b2a-8ee4-6b66ab82103a",
          "name": "createCachediSCSIVolume",
          "request": {
            "url": "http://example.com/api/?Action=CreateCachediSCSIVolume?ClientToken=ClientToken&GatewayARN=GatewayARN&NetworkInterfaceId=NetworkInterfaceId&SnapshotId=SnapshotId&SourceVolumeARN=SourceVolumeARN&TargetName=TargetName&VolumeSizeInBytes=VolumeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a cached volume on a specified cached gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84b5b873-ad98-497c-8b2f-ff5aa450cfc1"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Share",
      "item": [
        {
          "id": "8480b644-ddaf-4222-bcb9-0eb4fc9b90cf",
          "name": "createNFSFileShare",
          "request": {
            "url": "http://example.com/api/?Action=CreateNFSFileShare?ClientToken=ClientToken&DefaultStorageClass=DefaultStorageClass&GatewayARN=GatewayARN&KMSEncrypted=KMSEncrypted&KMSKey=KMSKey&LocationARN=LocationARN&NFSFileShareDefaults=NFSFileShareDefaults&Role=Role",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a file share on an existing file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c352c1f8-b5bb-4337-8f0c-6d2d177f240c"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "285afed6-6782-47cf-8400-55b0962e2d0c",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?SnapshotDescription=SnapshotDescription&VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a snapshot of a volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3653ef0b-1dfc-4866-b7f1-1be226347b1b"
            }
          ]
        },
        {
          "id": "9e28c72b-ea85-42bb-876f-bd3c0dcc8c1c",
          "name": "createSnapshotFromVolumeRecoveryPoint",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshotFromVolumeRecoveryPoint?SnapshotDescription=SnapshotDescription&VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a snapshot of a gateway from a volume recovery point."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c78780d-d536-4343-9ced-bb731389e6d3"
            }
          ]
        },
        {
          "id": "74032f06-583b-4b36-9a02-27e9b60da661",
          "name": "deleteSnapshotSchedule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshotSchedule?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a snapshot of a volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12802697-5f36-437f-bfce-3dd13d5287d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volume",
      "item": [
        {
          "id": "d71a73bc-9ede-4034-97c4-51435bc6cdf3",
          "name": "createStorediSCSIVolume",
          "request": {
            "url": "http://example.com/api/?Action=CreateStorediSCSIVolume?DiskId=DiskId&GatewayARN=GatewayARN&NetworkInterfaceId=NetworkInterfaceId&PreserveExistingData=PreserveExistingData&SnapshotId=SnapshotId&TargetName=TargetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a volume on a specified gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "537e1763-d95a-4c9a-9c7f-6e0ee4d18333"
            }
          ]
        }
      ]
    },
    {
      "name": "Tapes",
      "item": [
        {
          "id": "5011c6b6-9fa9-4765-9046-14245bd717fe",
          "name": "createTapes",
          "request": {
            "url": "http://example.com/api/?Action=CreateTapes?ClientToken=ClientToken&GatewayARN=GatewayARN&NumTapesToCreate=NumTapesToCreate&TapeBarcodePrefix=TapeBarcodePrefix&TapeSizeInBytes=TapeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates one or more virtual tapes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d61f4afb-bb12-4118-9338-0d693075e5ec"
            }
          ]
        },
        {
          "id": "61a997cb-05e3-4298-89b8-7b4cedfbb30a",
          "name": "deleteTape",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTape?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified virtual tape."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4851aede-645e-4552-a2ed-0ac07973eef4"
            }
          ]
        },
        {
          "id": "b5bffdd9-abe6-47c3-853d-c9271bfa490d",
          "name": "deleteTapeArchive",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTapeArchive?TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified virtual tape from the virtual tape shelf (VTS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aed853c3-6e09-4c5e-aa11-3a53a12ecd28"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape With Barcode",
      "item": [
        {
          "id": "d5a2055f-504a-4a71-b5da-c23972902578",
          "name": "createTapeWithBarcode",
          "request": {
            "url": "http://example.com/api/?Action=CreateTapeWithBarcode?GatewayARN=GatewayARN&TapeBarcode=TapeBarcode&TapeSizeInBytes=TapeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a virtual tape by using your own barcode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8db3f4a7-5188-42ee-8c60-79d6ddc1a7ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Bandwidth Rate Limit",
      "item": [
        {
          "id": "1f64e680-c228-49aa-806a-30ecc11a843e",
          "name": "deleteBandwidthRateLimit",
          "request": {
            "url": "http://example.com/api/?Action=DeleteBandwidthRateLimit?BandwidthType=BandwidthType&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the bandwidth rate limits of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b6c5485-36a4-4fde-b181-08d86dd1d0ef"
            }
          ]
        },
        {
          "id": "a1f41aa2-c247-4cd9-b93c-ccdcb8c15499",
          "name": "describeBandwidthRateLimit",
          "request": {
            "url": "http://example.com/api/?Action=DescribeBandwidthRateLimit?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the bandwidth rate limits of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24c58184-5161-4454-bd51-8b6e1e9a7a24"
            }
          ]
        }
      ]
    },
    {
      "name": "Chap Credentials",
      "item": [
        {
          "id": "27ae5472-6a21-4e85-96c0-46ce50877fbb",
          "name": "deleteChapCredentials",
          "request": {
            "url": "http://example.com/api/?Action=DeleteChapCredentials?InitiatorName=InitiatorName&TargetARN=TargetARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes Challenge-Handshake Authentication Protocol (CHAP) credentials for a\n         specified iSCSI target and initiator pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe13a3fc-e944-4a9c-bc22-979ebd71177d"
            }
          ]
        }
      ]
    },
    {
      "name": "File Share",
      "item": [
        {
          "id": "bcc115ce-49be-4c1e-8904-c8575215be23",
          "name": "deleteFileShare",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFileShare?FileShareARN=FileShareARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a file share from a file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0e3f338-08ca-430d-8302-b6eb5349b12a"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "ddfd3ff0-8d95-48b2-85c5-16c000c76a2d",
          "name": "deleteVolume",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVolume?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified gateway volume that you previously created using the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4355dfe9-1b95-4972-8f84-a0be74dc6f63"
            }
          ]
        }
      ]
    }
  ]
}