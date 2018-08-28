---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Describe Maintenance Start Time
  version: 1.0.0
  description: |-
    Returns your gateway's weekly maintenance start time including the day and time of
             the week.
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