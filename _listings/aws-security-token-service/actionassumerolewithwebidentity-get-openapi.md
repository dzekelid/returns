---
swagger: "2.0"
x-collection-name: AWS Security Token Service
x-complete: 0
info:
  title: AWS Security Token Service API Assume Role With Web Identity
  version: 1.0.0
  description: |-
    Returns a set of temporary security credentials for users who have been authenticated
          in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,
          Facebook, Google, or any OpenID Connect-compatible identity provider.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssumeRole:
    get:
      summary: Assume Role
      description: |-
        Returns a set of temporary security credentials (consisting of an access key ID, a
              secret access key, and a security token) that you can use to access AWS resources that you
              might not normally have access to.
      operationId: assumeRole
      x-api-path-slug: actionassumerole-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, of the role session
        type: string
      - in: query
        name: ExternalId
        description: A unique identifier that is used by third parties when assuming
          roles in their      customers accounts
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the role to assume
        type: string
      - in: query
        name: RoleSessionName
        description: An identifier for the assumed role session
        type: string
      - in: query
        name: SerialNumber
        description: The identification number of the MFA device that is associated
          with the user who is      making the AssumeRole call
        type: string
      - in: query
        name: TokenCode
        description: The value provided by the MFA device, if the trust policy of
          the role being assumed      requires MFA (that is, if the policy includes
          a condition that tests for MFA)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=AssumeRoleWithSAML:
    get:
      summary: Assume Role With S A M L
      description: |-
        Returns a set of temporary security credentials for users who have been authenticated
              via a SAML authentication response.
      operationId: assumeRoleWithSAML
      x-api-path-slug: actionassumerolewithsaml-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, of the role session
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format
        type: string
      - in: query
        name: PrincipalArn
        description: The Amazon Resource Name (ARN) of the SAML provider in IAM that
          describes the      IdP
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the role that the caller is
          assuming
        type: string
      - in: query
        name: SAMLAssertion
        description: The base-64 encoded SAML authentication response provided by
          the IdP
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=AssumeRoleWithWebIdentity:
    get:
      summary: Assume Role With Web Identity
      description: |-
        Returns a set of temporary security credentials for users who have been authenticated
              in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,
              Facebook, Google, or any OpenID Connect-compatible identity provider.
      operationId: assumeRoleWithWebIdentity
      x-api-path-slug: actionassumerolewithwebidentity-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, of the role session
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format
        type: string
      - in: query
        name: ProviderId
        description: The fully qualified host component of the domain name of the
          identity      provider
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the role that the caller is
          assuming
        type: string
      - in: query
        name: RoleSessionName
        description: An identifier for the assumed role session
        type: string
      - in: query
        name: WebIdentityToken
        description: The OAuth 2
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
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