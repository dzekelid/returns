---
swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 0
info:
  title: AWS Key Management Service API List Retirable Grants
  version: 1.0.0
  description: |-
    Returns a list of all grants for which the grant's RetiringPrincipal
          matches the one specified.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GenerateDataKey:
    get:
      summary: Generate Data Key
      description: |-
        Returns a data encryption key that you can use in your application to encrypt
              data locally.
      operationId: generateDataKey
      x-api-path-slug: actiongeneratedatakey-get
      parameters:
      - in: query
        name: EncryptionContext
        description: A set of key-value pairs that represents additional authenticated
          data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK under which to generate and encrypt
          the data encryption      key
        type: string
      - in: query
        name: KeySpec
        description: The length of the data encryption key
        type: string
      - in: query
        name: NumberOfBytes
        description: The length of the data encryption key in bytes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GenerateDataKeyWithoutPlaintext:
    get:
      summary: Generate Data Key Without Plaintext
      description: Returns a data encryption key encrypted under a customer master
        key (CMK).
      operationId: generateDataKeyWithoutPlaintext
      x-api-path-slug: actiongeneratedatakeywithoutplaintext-get
      parameters:
      - in: query
        name: EncryptionContext
        description: A set of key-value pairs that represents additional authenticated
          data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK under which to generate and encrypt
          the data encryption      key
        type: string
      - in: query
        name: KeySpec
        description: The length of the data encryption key
        type: string
      - in: query
        name: NumberOfBytes
        description: The length of the data encryption key in bytes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GetParametersForImport:
    get:
      summary: Get Parameters For Import
      description: |-
        Returns the items you need in order to import key material into AWS KMS from your
              existing key management infrastructure.
      operationId: getParametersForImport
      x-api-path-slug: actiongetparametersforimport-get
      parameters:
      - in: query
        name: KeyId
        description: The identifier of the CMK into which you will import key material
        type: string
      - in: query
        name: WrappingAlgorithm
        description: The algorithm you will use to encrypt the key material before
          importing it with ImportKeyMaterial
        type: string
      - in: query
        name: WrappingKeySpec
        description: The type of wrapping key (public key) to return in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=ListRetirableGrants:
    get:
      summary: List Retirable Grants
      description: |-
        Returns a list of all grants for which the grant's RetiringPrincipal
              matches the one specified.
      operationId: listRetirableGrants
      x-api-path-slug: actionlistretirablegrants-get
      parameters:
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      - in: query
        name: RetiringPrincipal
        description: The retiring principal for which to list grants
        type: string
      responses:
        200:
          description: OK
      tags:
      - Grants
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