---
name: AWS Direct Connect
x-slug: aws-direct-connect
description: AWS Direct Connect makes it easy to establish a dedicated network connection
  from your premises to AWS. Using AWS Direct Connect, you can establish private connectivity
  between AWS and your datacenter, office, or colocation environment, which in many
  cases can reduce your network costs, increase bandwidth throughput, and provide
  a more consistent network experience than Internet-based connections.AWS Direct
  Connect lets you establish a dedicated network connection between your network and
  one of the AWS Direct Connect locations. Using industry standard 802.1q VLANs, this
  dedicated connection can be partitioned into multiple virtual interfaces. This allows
  you to use the same connection to access public resources such as objects stored
  in Amazon S3 using public IP address space, and private resources such as Amazon
  EC2 instances running within anAmazon Virtual Private Cloud (VPC)using private IP
  space, while maintaining network separation between the public and private environments.
  Virtual interfaces can be reconfigured at any time to meet your changing needs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AWSDirectConnect.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Direct Connect API - Describe Connection Loa
  x-api-slug: actiondescribeconnectionloa-get
  description: Returns the LOA-CFA for a Connection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AWSDirectConnect.png
  humanURL: https://aws.amazon.com/directconnect/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Profiles, Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribeconnectionloa-get-openapi.md
- name: AWS Direct Connect API - Describe Connections On Interconnect
  x-api-slug: actiondescribeconnectionsoninterconnect-get
  description: Return a list of connections that have been provisioned on the given
    interconnect.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AWSDirectConnect.png
  humanURL: https://aws.amazon.com/directconnect/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Profiles, Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribeconnectionsoninterconnect-get-openapi.md
- name: AWS Direct Connect API - Describe Interconnect Loa
  x-api-slug: actiondescribeinterconnectloa-get
  description: Returns the LOA-CFA for an Interconnect.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AWSDirectConnect.png
  humanURL: https://aws.amazon.com/directconnect/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Profiles, Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribeinterconnectloa-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribeinterconnectloa-get-openapi.md
- name: AWS Direct Connect API - Describe Interconnects
  x-api-slug: actiondescribeinterconnects-get
  description: Returns a list of interconnects owned by the AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AWSDirectConnect.png
  humanURL: https://aws.amazon.com/directconnect/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Profiles, Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribeinterconnects-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribeinterconnects-get-openapi.md
- name: AWS Direct Connect API - Describe Locations
  x-api-slug: actiondescribelocations-get
  description: Returns the list of AWS Direct Connect locations in the current AWS
    region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AWSDirectConnect.png
  humanURL: https://aws.amazon.com/directconnect/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Profiles, Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribelocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribelocations-get-openapi.md
- name: AWS Direct Connect API - Describe Virtual Gateways
  x-api-slug: actiondescribevirtualgateways-get
  description: Returns a list of virtual private gateways owned by the AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AWSDirectConnect.png
  humanURL: https://aws.amazon.com/directconnect/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, API Service Provider, API Service Provider,
    API Provider, Profiles, Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-direct-connect/actiondescribevirtualgateways-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.device.farm.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.direct.connect.stack.network
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/AWS-Direct-Connect
- type: x-console
  url: https://console.aws.amazon.com/directconnect/
- type: x-documentation
  url: http://docs.aws.amazon.com/directconnect/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/directconnect/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=126
- type: x-getting-started
  url: https://aws.amazon.com/directconnect/getting-started/
- type: x-partner-bundles
  url: ttps://aws.amazon.com/directconnect/directconnectbundles/
- type: x-partners
  url: https://aws.amazon.com/directconnect/partners/
- type: x-pricing
  url: https://aws.amazon.com/directconnect/pricing/
- type: x-website
  url: https://aws.amazon.com/directconnect/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---