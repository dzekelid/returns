---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Domains
  version: 1.0.0
  description: Returns a list of all domains in the user's account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetActiveNames:
    get:
      summary: Get Active Names
      description: Returns the names of all active (not deleted) resources.
      operationId: getActiveNames
      x-api-path-slug: actiongetactivenames-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for paginating results from your get active names
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Names
  /?Action=GetBlueprints:
    get:
      summary: Get Blueprints
      description: Returns the list of available instance images, or blueprints.
      operationId: getBlueprints
      x-api-path-slug: actiongetblueprints-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value indicating whether to include inactive results
          in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get blueprints      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetBundles:
    get:
      summary: Get Bundles
      description: Returns the list of bundles that are available for purchase.
      operationId: getBundles
      x-api-path-slug: actiongetbundles-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value that indicates whether to include inactive bundle
          results in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get bundles      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundles
  /?Action=GetDomain:
    get:
      summary: Get Domain
      description: Returns information about a specific domain recordset.
      operationId: getDomain
      x-api-path-slug: actiongetdomain-get
      parameters:
      - in: query
        name: domainName
        description: The domain name for which your want to return information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=GetDomains:
    get:
      summary: Get Domains
      description: Returns a list of all domains in the user's account.
      operationId: getDomains
      x-api-path-slug: actiongetdomains-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get domains      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
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