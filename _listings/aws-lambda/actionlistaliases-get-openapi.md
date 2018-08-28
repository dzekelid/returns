---
swagger: "2.0"
x-collection-name: AWS Lambda
x-complete: 0
info:
  title: AWS Lambda API List Aliases
  version: 1.0.0
  description: Returns list of aliases created for a Lambda function.
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
  /?Action=GetFunctionConfiguration:
    get:
      summary: Get Function Configuration
      description: Returns the configuration information of the Lambda function.
      operationId: getFunctionConfiguration
      x-api-path-slug: actiongetfunctionconfiguration-get
      parameters:
      - in: query
        name: FunctionName
        description: The name of the Lambda function for which you want to retrieve
          the configuration information
        type: string
      - in: query
        name: Qualifier
        description: Using this optional parameter you can specify a function version
          or an alias name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Functions
  /?Action=GetPolicy:
    get:
      summary: Get Policy
      description: Returns the resource policy associated with the specified Lambda
        function.
      operationId: getPolicy
      x-api-path-slug: actiongetpolicy-get
      parameters:
      - in: query
        name: FunctionName
        description: Function name whose resource policy you want to retrieve
        type: string
      - in: query
        name: Qualifier
        description: You can specify this optional query parameter to specify a function
          version or an alias name in which case this API will return all permissions
          associated with the specific qualified ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=ListAliases:
    get:
      summary: List Aliases
      description: Returns list of aliases created for a Lambda function.
      operationId: listAliases
      x-api-path-slug: actionlistaliases-get
      parameters:
      - in: query
        name: FunctionName
        description: Lambda function name for which the alias is created
        type: string
      - in: query
        name: FunctionVersion
        description: If you specify this optional parameter, the API returns only
          the aliases that are pointing to the specific Lambda function version, otherwise
          the API returns all of the aliases created for the Lambda function
        type: string
      - in: query
        name: Marker
        description: Optional string
        type: string
      - in: query
        name: MaxItems
        description: Optional integer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aliases
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