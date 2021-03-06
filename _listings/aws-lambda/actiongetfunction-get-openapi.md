---
swagger: "2.0"
x-collection-name: AWS Lambda
x-complete: 0
info:
  title: AWS Lambda API Get Function
  version: 1.0.0
  description: "Returns the configuration information of the Lambda function and a
    presigned URL \n      link to the."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetAccountSettings:
    get:
      summary: Get Account Settings
      description: Returns a customer's account settings.
      operationId: getAccountSettings
      x-api-path-slug: actiongetaccountsettings-get
      parameters:
      - in: query
        name: AccountLimit
        description: Provides limits of code size and concurrency associated with
          the current account and region
        type: string
      - in: query
        name: AccountUsage
        description: Provides code size usage and function count associated with the
          current account and region
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /?Action=GetAlias:
    get:
      summary: Get Alias
      description: "Returns the specified alias information such as the alias ARN,
        description, and function version it \n      is pointing to."
      operationId: getAlias
      x-api-path-slug: actiongetalias-get
      parameters:
      - in: query
        name: FunctionName
        description: Function name for which the alias is created
        type: string
      - in: query
        name: Name
        description: Name of the alias for which you want to retrieve information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aliases
  /?Action=GetEventSourceMapping:
    get:
      summary: Get Event Source Mapping
      description: Returns configuration information for the specified event source
        mapping (see.
      operationId: getEventSourceMapping
      x-api-path-slug: actiongeteventsourcemapping-get
      parameters:
      - in: query
        name: UUID
        description: The AWS Lambda assigned ID of the event source mapping
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Sources
  /?Action=GetFunction:
    get:
      summary: Get Function
      description: "Returns the configuration information of the Lambda function and
        a presigned URL \n      link to the."
      operationId: getFunction
      x-api-path-slug: actiongetfunction-get
      parameters:
      - in: query
        name: FunctionName
        description: The Lambda function name
        type: string
      - in: query
        name: Qualifier
        description: Using this optional parameter to specify a function version or
          an alias name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Functions
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