---
name: AWS Key Management Service
x-slug: aws-key-management-service
description: AWS Key Management Service (KMS) is a managed service that makes it easy
  for you to create and control the encryption keys used to encrypt your data, and
  uses Hardware Security Modules (HSMs) to protect the security of your keys. AWS
  Key Management Service is integrated with several other AWS services to help you
  protect the data you store with these services. AWS Key Management Service is also
  integrated with AWS CloudTrail to provide you with logs of all key usage to help
  meet your regulatory and compliance needs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
x-kinRank: "10"
x-alexaRank: "0"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-key-management-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Key Management Service API - Generate Data Key
  x-api-slug: actiongeneratedatakey-get
  description: |-
    Returns a data encryption key that you can use in your application to encrypt
          data locally.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-key-management-service/actiongeneratedatakey-get-openapi.md
- name: AWS Key Management Service API - Generate Data Key Without Plaintext
  x-api-slug: actiongeneratedatakeywithoutplaintext-get
  description: Returns a data encryption key encrypted under a customer master key
    (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-key-management-service/actiongeneratedatakeywithoutplaintext-get-openapi.md
- name: AWS Key Management Service API - Get Parameters For Import
  x-api-slug: actiongetparametersforimport-get
  description: |-
    Returns the items you need in order to import key material into AWS KMS from your
          existing key management infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-key-management-service/actiongetparametersforimport-get-openapi.md
- name: AWS Key Management Service API - List Retirable Grants
  x-api-slug: actionlistretirablegrants-get
  description: |-
    Returns a list of all grants for which the grant's RetiringPrincipal
          matches the one specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-key-management-service/actionlistretirablegrants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-key-management-service/actionlistretirablegrants-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.internet.of.things.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.key.management.service.stack.network
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/kms/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/kms/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/kms/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/kms/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/kms/pricing/
- type: x-website
  url: https://aws.amazon.com/kms/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---