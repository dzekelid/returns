---
name: AWS Storage Gateway Service
x-slug: aws-storage-gateway-service
description: The AWS Storage Gateway service seamlessly enables hybrid storage between
  on-premises storage environments andthe AWS Cloud. It combines a multi-protocol
  storage appliance with highly efficient network connectivity toAmazon cloud storageservices,
  delivering local performance with virtually unlimited scale. Customers use it in
  remote offices and datacenters for hybrid cloud workloads, backup and restore, archive,
  disaster recovery, and tiered storage.The Storage Gateway virtual appliance connects
  seamlessly to your local infrastructure as a file server, as a volume, or as a virtual
  tape library (VTL). This seamless connection makes it simple for organizations to
  augment existing on-premises storage investments with the high scalability, extreme
  durability and low cost of cloud storage.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Storage Gateway Service API - Describe Bandwidth Rate Limit
  x-api-slug: actiondescribebandwidthratelimit-get
  description: Returns the bandwidth rate limits of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribebandwidthratelimit-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribebandwidthratelimit-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Cache
  x-api-slug: actiondescribecache-get
  description: Returns information about the cache of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribecache-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribecache-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Cached SCSI Volumes
  x-api-slug: actiondescribecachediscsivolumes-get
  description: Returns a description of the gateway volumes specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribecachediscsivolumes-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Chap Credentials
  x-api-slug: actiondescribechapcredentials-get
  description: |-
    Returns an array of Challenge-Handshake Authentication Protocol (CHAP) credentials
             information for a specified iSCSI target, one for each target-initiator pair.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribechapcredentials-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribechapcredentials-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Gateway Information
  x-api-slug: actiondescribegatewayinformation-get
  description: |-
    Returns metadata about a gateway such as its name, network interfaces, configured
             time zone, and the state (whether the gateway is running or not).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribegatewayinformation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribegatewayinformation-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Maintenance Start Time
  x-api-slug: actiondescribemaintenancestarttime-get
  description: |-
    Returns your gateway's weekly maintenance start time including the day and time of
             the week.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribemaintenancestarttime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribemaintenancestarttime-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Stored SCSI Volumes
  x-api-slug: actiondescribestorediscsivolumes-get
  description: Returns the description of the gateway volumes specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribestorediscsivolumes-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Tape Archives
  x-api-slug: actiondescribetapearchives-get
  description: |-
    Returns a description of specified virtual tapes in the virtual tape shelf
             (VTS).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribetapearchives-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Tape Recovery Points
  x-api-slug: actiondescribetaperecoverypoints-get
  description: |-
    Returns a list of virtual tape recovery points that are available for the specified
             gateway-VTL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribetaperecoverypoints-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Tapes
  x-api-slug: actiondescribetapes-get
  description: Returns a description of the specified Amazon Resource Name (ARN) of
    virtual tapes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribetapes-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Upload Buffer
  x-api-slug: actiondescribeuploadbuffer-get
  description: Returns information about the upload buffer of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribeuploadbuffer-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribeuploadbuffer-get-openapi.md
- name: AWS Storage Gateway Service API - Describe VTL Devices
  x-api-slug: actiondescribevtldevices-get
  description: |-
    Returns a description of virtual tape library (VTL) devices for the specified
             gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribevtldevices-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Working Storage
  x-api-slug: actiondescribeworkingstorage-get
  description: Returns information about the working storage of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actiondescribeworkingstorage-get-openapi.md
- name: AWS Storage Gateway Service API - List Local Disks
  x-api-slug: actionlistlocaldisks-get
  description: Returns a list of the gateway's local disks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-storage-gateway-service/actionlistlocaldisks-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.step.functions.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.storage.gateway.service.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/storagegateway/latest/APIReference
- type: x-faq
  url: https://aws.amazon.com/storagegateway/faqs/
- type: x-pricing
  url: https://aws.amazon.com/storagegateway/pricing/
- type: x-website
  url: https://aws.amazon.com/storagegateway/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---