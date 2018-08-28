---
name: AWS Identity and Access Management
x-slug: aws-identity-and-access-management
description: AWS Identity and Access Management (IAM) enables you to securely control
  access to AWS services and resources for your users. Using IAM, you can create and
  manage AWS users and groups, and use permissions to allow and deny their access
  to AWS resources.IAM is a feature of your AWS account offered at no additional charge.
  You will be charged only for use of other AWS services by your users.To get started
  using IAM, orif you have already registered with AWS, go to theAWS Management Consoleand
  get started with theseIAM Best Practices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Identity and Access Management API - Get Group
  x-api-slug: actiongetgroup-get
  description: Returns a list of IAM users that are in the specified IAM group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Amazon Web Services, Authentication, Stack Network, Security, API Service
    Provider, API Service Provider, API Provider, Identities, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actiongetgroup-get-openapi.md
- name: AWS Identity and Access Management API - Get Open I D Connect Provider
  x-api-slug: actiongetopenidconnectprovider-get
  description: |-
    Returns information about the specified OpenID Connect (OIDC) provider resource object
          in IAM.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Amazon Web Services, Authentication, Stack Network, Security, API Service
    Provider, API Service Provider, API Provider, Identities, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actiongetopenidconnectprovider-get-openapi.md
- name: AWS Identity and Access Management API - Get S A M L Provider
  x-api-slug: actiongetsamlprovider-get
  description: |-
    Returns the SAML provider metadocument that was uploaded when the IAM SAML provider
          resource object was created or updated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Amazon Web Services, Authentication, Stack Network, Security, API Service
    Provider, API Service Provider, API Provider, Identities, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actiongetsamlprovider-get-openapi.md
- name: AWS Identity and Access Management API - List Access Keys
  x-api-slug: actionlistaccesskeys-get
  description: Returns information about the access key IDs associated with the specified
    IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Amazon Web Services, Authentication, Stack Network, Security, API Service
    Provider, API Service Provider, API Provider, Identities, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actionlistaccesskeys-get-openapi.md
- name: AWS Identity and Access Management API - List Service Specific Credentials
  x-api-slug: actionlistservicespecificcredentials-get
  description: |-
    Returns information about the service-specific credentials associated with the
          specified IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Amazon Web Services, Authentication, Stack Network, Security, API Service
    Provider, API Service Provider, API Provider, Identities, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actionlistservicespecificcredentials-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actionlistservicespecificcredentials-get-openapi.md
- name: AWS Identity and Access Management API - List Signing Certificates
  x-api-slug: actionlistsigningcertificates-get
  description: |-
    Returns information about the signing certificates associated with the specified IAM
          user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Amazon Web Services, Authentication, Stack Network, Security, API Service
    Provider, API Service Provider, API Provider, Identities, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actionlistsigningcertificates-get-openapi.md
- name: AWS Identity and Access Management API - List S S H Public Keys
  x-api-slug: actionlistsshpublickeys-get
  description: Returns information about the SSH public keys associated with the specified
    IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Amazon Web Services, Authentication, Stack Network, Security, API Service
    Provider, API Service Provider, API Provider, Identities, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-identity-and-access-management/actionlistsshpublickeys-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.glacier.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.identity.and.access.management.stack.network
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=323
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/sts/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/IAM/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/iam/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=76
- type: x-getting-started
  url: https://aws.amazon.com/iam/getting-started/
- type: x-partners
  url: https://aws.amazon.com/iam/partners/
- type: x-tools
  url: http://aws.amazon.com/cli
- type: x-website
  url: https://aws.amazon.com/iam/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---