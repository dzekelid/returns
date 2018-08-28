---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Framework Get an analytic catalog entry by id.
  version: 1.0.0
  description: Returns the analytic catalog entry with the given id.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/policy-evaluation:
    post:
      summary: Evaluates all applicable policies and returns decision result
      description: Evaluates all applicable policies and returns decision result.
      operationId: evalPolicyV1UsingPOST
      x-api-path-slug: v1policyevaluation-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Evaluates
      - ""
      - Applicable
      - Policies
      - Returns
      - Decision
      - Result
  /v1/policy-set:
    get:
      summary: Returns all the policy sets for the given zone.
      description: Returns all the policy sets for the given zone..
      operationId: getAllPolicySetsUsingGET_1
      x-api-path-slug: v1policyset-get
      responses:
        200:
          description: Successful response
      tags:
      - Returns
      - ""
      - Policy
      - Setsthe
      - Given
      - Zone
  /api/v1/analytic/execution/async/{requestId}/result:
    get:
      summary: Get the analytic execution result by request id.
      description: Returns the analytic execution result.
      operationId: retrieveAnalyticExecutionResult
      x-api-path-slug: apiv1analyticexecutionasyncrequestidresult-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: path
        name: requestId
        description: analytic execution request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Execution
      - Result
      - By
      - Request
      - Id
  /api/v1/analytic/execution/async/{requestId}/status:
    get:
      summary: Get the analytic execution status by request id.
      description: Returns the analytic execution status (one of QUEUED, PROCESSING,
        COMPLETED, or FAILED).
      operationId: retrieveAnalyticExecutionStatus
      x-api-path-slug: apiv1analyticexecutionasyncrequestidstatus-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: path
        name: requestId
        description: analytic execution request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Execution
      - Status
      - By
      - Request
      - Id
  /api/v1/catalog/analytics:
    get:
      summary: Get all analytic catalog entries.
      description: Returns all analytic catalog entries as specified by page and sort
        criteria.
      operationId: retrieveAll
      x-api-path-slug: apiv1cataloganalytics-get
      parameters:
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortableFields
        description: 'sortable fields : name'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      - in: query
        name: taxonomyPath
        description: 'taxonomy path : taxonomyPath'
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entries
  /api/v1/catalog/analytics/versions:
    get:
      summary: Get all versions of the analytic catalog entry with the given name.
      description: Returns all versions of the analytic catalog entry with the given
        name.
      operationId: retrieveByName
      x-api-path-slug: apiv1cataloganalyticsversions-get
      parameters:
      - in: query
        name: name
        description: analytic name
      responses:
        2:
          description: Successful response
      tags:
      - Versions
      - Of
      - Analytic
      - Catalog
      - Entry
      - Given
      - Name
  /api/v1/catalog/analytics/{id}:
    get:
      summary: Get an analytic catalog entry by id.
      description: Returns the analytic catalog entry with the given id.
      operationId: retrieveAnalyticCatalogEntryById
      x-api-path-slug: apiv1cataloganalyticsid-get
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entry
      - By
      - Id
  /api/v1/catalog/analytics/{id}/artifacts:
    get:
      summary: Get the descriptive information of the artifacts corresponding to an
        analytic catalog entry.
      description: 'Returns the description information (type, description, etc.)
        for all artifacts associated with the given analytic catalog entry id. Note:
        it does not return the artifact file contents; use the download APIs to obtain
        an artifact file. An error is returned if the supplied analytic catalog entry
        id does not exist.'
      operationId: retrieveArtifactsByCatalogEntryId
      x-api-path-slug: apiv1cataloganalyticsidartifacts-get
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        200:
          description: OK
      tags:
      - Descriptive
      - Information
      - Of
      - Artifacts
      - Corresponding
      - To
      - Analytic
      - Catalog
      - Entry
  /api/v1/catalog/analytics/{id}/deployment/{requestId}:
    get:
      summary: Get the analytic deployment status by request id.
      description: Returns the analytic deployment status (one of 'queued,' 'processing,'
        or 'completed').
      operationId: retrieveAnalyticDeploymentResult
      x-api-path-slug: apiv1cataloganalyticsiddeploymentrequestid-get
      parameters:
      - in: path
        name: id
        description: analytic id
      - in: path
        name: requestId
        description: analytic deployment request id
      responses:
        200:
          description: OK
      tags:
      - Analytic
      - Deployment
      - Status
      - By
      - Request
      - Id
  /api/v1/catalog/analytics/{id}/logs:
    get:
      summary: Get the analytic recent logs
      description: Return the recent analytic logs
      operationId: retrieveAnalyticLog
      x-api-path-slug: apiv1cataloganalyticsidlogs-get
      parameters:
      - in: path
        name: id
        description: analytic id
      responses:
        200:
          description: OK
      tags:
      - Analytic
      - Recent
      - Logs
  /api/v1/catalog/analytics/{id}/validation/{validationRequestId}:
    get:
      summary: Get the analytic validation status by validation request id.
      description: Returns the analytic validation status (one of 'queued,' 'processing,'
        or 'completed' and the result from running the analytic (when status is 'completed').
      operationId: retrieveAnalyticValidationResult
      x-api-path-slug: apiv1cataloganalyticsidvalidationvalidationrequestid-get
      parameters:
      - in: path
        name: id
        description: analytic id
      - in: path
        name: validationRequestId
        description: analytic validation request id
      responses:
        200:
          description: OK
      tags:
      - Analytic
      - Validation
      - Status
      - By
      - Validation
      - Request
      - Id
  /api/v1/analytics/customdata/read:
    post:
      summary: Retrieve analytic input data from custom datasource.
      description: Returns the analytic input data used during runtime execution.
      operationId: readCustomProviderData
      x-api-path-slug: apiv1analyticscustomdataread-post
      parameters:
      - in: body
        name: body
        description: Analytic Input Data Read request
        schema:
          $ref: '#/definitions/holder'
      responses:
        2:
          description: Successful response
      tags:
      - Retrieve
      - Analytic
      - Input
      - Data
      - From
      - Custom
      - Datasource
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