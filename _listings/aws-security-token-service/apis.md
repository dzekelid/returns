---
name: AWS Security Token Service
x-slug: aws-security-token-service
description: The AWS Security Token Service (STS) is a web service that enables you
  to request temporary, limited-privilege credentials for AWS Identity and Access
  Management (IAM) users or for users that you authenticate (federated users).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Security Token Service API - Assume Role
  x-api-slug: actionassumerole-get
  description: |-
    Returns a set of temporary security credentials (consisting of an access key ID, a
          secret access key, and a security token) that you can use to access AWS resources that you
          might not normally have access to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
  humanURL: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
  baseURL: :///
  tags: Amazon Web Services, Authentication, Security, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actionassumerole-get-openapi.md
- name: AWS Security Token Service API - Assume Role With S A M L
  x-api-slug: actionassumerolewithsaml-get
  description: |-
    Returns a set of temporary security credentials for users who have been authenticated
          via a SAML authentication response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
  humanURL: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
  baseURL: :///
  tags: Amazon Web Services, Authentication, Security, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actionassumerolewithsaml-get-openapi.md
- name: AWS Security Token Service API - Assume Role With Web Identity
  x-api-slug: actionassumerolewithwebidentity-get
  description: |-
    Returns a set of temporary security credentials for users who have been authenticated
          in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,
          Facebook, Google, or any OpenID Connect-compatible identity provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
  humanURL: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
  baseURL: :///
  tags: Amazon Web Services, Authentication, Security, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actionassumerolewithwebidentity-get-openapi.md
- name: AWS Security Token Service API - Get Caller Identity
  x-api-slug: actiongetcalleridentity-get
  description: |-
    Returns details about the IAM identity whose credentials are used to call the
          API.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
  humanURL: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
  baseURL: :///
  tags: Amazon Web Services, Authentication, Security, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actiongetcalleridentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actiongetcalleridentity-get-openapi.md
- name: AWS Security Token Service API - Get Federation Token
  x-api-slug: actiongetfederationtoken-get
  description: |-
    Returns a set of temporary security credentials (consisting of an access key ID, a
          secret access key, and a security token) for a federated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
  humanURL: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
  baseURL: :///
  tags: Amazon Web Services, Authentication, Security, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actiongetfederationtoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actiongetfederationtoken-get-openapi.md
- name: AWS Security Token Service API - Get Session Token
  x-api-slug: actiongetsessiontoken-get
  description: Returns a set of temporary credentials for an AWS account or IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM_AWSSTS.png
  humanURL: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
  baseURL: :///
  tags: Amazon Web Services, Authentication, Security, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actiongetsessiontoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/aws-security-token-service/actiongetsessiontoken-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.s3.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.security.token.service.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/STS/latest/APIReference/
- type: x-errors
  url: http://docs.aws.amazon.com/STS/latest/APIReference/CommonErrors.html
- type: x-website
  url: http://docs.aws.amazon.com/STS/latest/APIReference/Welcome.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---