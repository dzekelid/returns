swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetGroup:
    get:
      summary: Get Group
      description: Returns a list of IAM users that are in the specified IAM group.
      operationId: getGroup
      x-api-path-slug: actiongetgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=GetOpenIDConnectProvider:
    get:
      summary: Get Open I D Connect Provider
      description: |-
        Returns information about the specified OpenID Connect (OIDC) provider resource object
              in IAM.
      operationId: getOpenIDConnectProvider
      x-api-path-slug: actiongetopenidconnectprovider-get
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the OIDC provider resource
          object in IAM to get      information for
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=GetSAMLProvider:
    get:
      summary: Get S A M L Provider
      description: |-
        Returns the SAML provider metadocument that was uploaded when the IAM SAML provider
              resource object was created or updated.
      operationId: getSAMLProvider
      x-api-path-slug: actiongetsamlprovider-get
      parameters:
      - in: query
        name: SAMLProviderArn
        description: The Amazon Resource Name (ARN) of the SAML provider resource
          object in IAM to get      information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - SAML Providers
  /?Action=ListAccessKeys:
    get:
      summary: List Access Keys
      description: Returns information about the access key IDs associated with the
        specified IAM user.
      operationId: listAccessKeys
      x-api-path-slug: actionlistaccesskeys-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=ListServiceSpecificCredentials:
    get:
      summary: List Service Specific Credentials
      description: |-
        Returns information about the service-specific credentials associated with the
              specified IAM user.
      operationId: listServiceSpecificCredentials
      x-api-path-slug: actionlistservicespecificcredentials-get
      parameters:
      - in: query
        name: ServiceName
        description: Filters the returned results to only those for the specified
          AWS service
        type: string
      - in: query
        name: UserName
        description: The name of the user whose service-specific credentials you want
          information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Specific Credentials
  /?Action=ListSigningCertificates:
    get:
      summary: List Signing Certificates
      description: |-
        Returns information about the signing certificates associated with the specified IAM
              user.
      operationId: listSigningCertificates
      x-api-path-slug: actionlistsigningcertificates-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user whose signing certificates you want
          to examine
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
  /?Action=ListSSHPublicKeys:
    get:
      summary: List S S H Public Keys
      description: Returns information about the SSH public keys associated with the
        specified IAM user.
      operationId: listSSHPublicKeys
      x-api-path-slug: actionlistsshpublickeys-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to list SSH public keys for
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Keys