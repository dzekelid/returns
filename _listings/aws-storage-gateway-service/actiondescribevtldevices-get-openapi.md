---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Describe VTL Devices
  version: 1.0.0
  description: |-
    Returns a description of virtual tape library (VTL) devices for the specified
             gateway.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeBandwidthRateLimit:
    get:
      summary: Describe Bandwidth Rate Limit
      description: Returns the bandwidth rate limits of a gateway.
      operationId: describeBandwidthRateLimit
      x-api-path-slug: actiondescribebandwidthratelimit-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bandwidth Rate Limit
  /?Action=DescribeCache:
    get:
      summary: Describe Cache
      description: Returns information about the cache of a gateway.
      operationId: describeCache
      x-api-path-slug: actiondescribecache-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
  /?Action=DescribeCachediSCSIVolumes:
    get:
      summary: Describe Cached SCSI Volumes
      description: Returns a description of the gateway volumes specified in the request.
      operationId: describeCachediSCSIVolumes
      x-api-path-slug: actiondescribecachediscsivolumes-get
      parameters:
      - in: query
        name: VolumeARNs
        description: 'Type: array of Strings'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cached SCSI Volumes
  /?Action=DescribeChapCredentials:
    get:
      summary: Describe Chap Credentials
      description: |-
        Returns an array of Challenge-Handshake Authentication Protocol (CHAP) credentials
                 information for a specified iSCSI target, one for each target-initiator pair.
      operationId: describeChapCredentials
      x-api-path-slug: actiondescribechapcredentials-get
      parameters:
      - in: query
        name: TargetARN
        description: The Amazon Resource Name (ARN) of the iSCSI volume target
        type: string
      responses:
        200:
          description: OK
      tags:
      - Chap Credentials
  /?Action=DescribeGatewayInformation:
    get:
      summary: Describe Gateway Information
      description: |-
        Returns metadata about a gateway such as its name, network interfaces, configured
                 time zone, and the state (whether the gateway is running or not).
      operationId: describeGatewayInformation
      x-api-path-slug: actiondescribegatewayinformation-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=DescribeMaintenanceStartTime:
    get:
      summary: Describe Maintenance Start Time
      description: |-
        Returns your gateway's weekly maintenance start time including the day and time of
                 the week.
      operationId: describeMaintenanceStartTime
      x-api-path-slug: actiondescribemaintenancestarttime-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
  /?Action=DescribeStorediSCSIVolumes:
    get:
      summary: Describe Stored SCSI Volumes
      description: Returns the description of the gateway volumes specified in the
        request.
      operationId: describeStorediSCSIVolumes
      x-api-path-slug: actiondescribestorediscsivolumes-get
      parameters:
      - in: query
        name: VolumeARNs
        description: An array of strings where each string represents the Amazon Resource
          Name (ARN) of a         stored volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stored SCSI Volumes
  /?Action=DescribeTapeArchives:
    get:
      summary: Describe Tape Archives
      description: |-
        Returns a description of specified virtual tapes in the virtual tape shelf
                 (VTS).
      operationId: describeTapeArchives
      x-api-path-slug: actiondescribetapearchives-get
      parameters:
      - in: query
        name: Limit
        description: Specifies that the number of virtual tapes descried be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing virtual         tapes
        type: string
      - in: query
        name: TapeARNs
        description: Specifies one or more unique Amazon Resource Names (ARNs) that
          represent the virtual         tapes you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape Archives
  /?Action=DescribeTapeRecoveryPoints:
    get:
      summary: Describe Tape Recovery Points
      description: |-
        Returns a list of virtual tape recovery points that are available for the specified
                 gateway-VTL.
      operationId: describeTapeRecoveryPoints
      x-api-path-slug: actiondescribetaperecoverypoints-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of virtual tape recovery points that
          are described be         limited to the specified number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing the virtual         tape recovery points
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape Recovery Points
  /?Action=DescribeTapes:
    get:
      summary: Describe Tapes
      description: Returns a description of the specified Amazon Resource Name (ARN)
        of virtual tapes.
      operationId: describeTapes
      x-api-path-slug: actiondescribetapes-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of virtual tapes described be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: A marker value, obtained in a previous call to DescribeTapes
        type: string
      - in: query
        name: TapeARNs
        description: Specifies one or more unique Amazon Resource Names (ARNs) that
          represent the virtual         tapes you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
  /?Action=DescribeUploadBuffer:
    get:
      summary: Describe Upload Buffer
      description: Returns information about the upload buffer of a gateway.
      operationId: describeUploadBuffer
      x-api-path-slug: actiondescribeuploadbuffer-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload Buffer
  /?Action=DescribeVTLDevices:
    get:
      summary: Describe VTL Devices
      description: |-
        Returns a description of virtual tape library (VTL) devices for the specified
                 gateway.
      operationId: describeVTLDevices
      x-api-path-slug: actiondescribevtldevices-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of VTL devices described be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing the VTL         devices
        type: string
      - in: query
        name: VTLDeviceARNs
        description: An array of strings, where each string represents the Amazon
          Resource Name (ARN) of a         VTL device
        type: string
      responses:
        200:
          description: OK
      tags:
      - VTL Devices
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---