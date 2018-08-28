swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeIdentity:
    get:
      summary: Describe Identity
      description: |-
        Returns metadata related to the given identity, including when the identity was
                 created and any associated linked logins.
      operationId: describeIdentity
      x-api-path-slug: actiondescribeidentity-get
      parameters:
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
  /?Action=DescribeUserPool:
    get:
      summary: Describe User Pool
      description: |-
        Returns the configuration information and metadata of the specified user
                    pool.
      operationId: describeUserPool
      x-api-path-slug: actiondescribeuserpool-get
      parameters:
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=GetCredentialsForIdentity:
    get:
      summary: Get Credentials For Identity
      description: Returns credentials for the provided identity ID.
      operationId: getCredentialsForIdentity
      x-api-path-slug: actiongetcredentialsforidentity-get
      parameters:
      - in: query
        name: CustomRoleArn
        description: The Amazon Resource Name (ARN) of the role to be assumed when
          multiple roles were         received in the token from the identity provider
        type: string
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider         tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities