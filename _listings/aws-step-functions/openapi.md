swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 1
info:
  title: AWS Step Functions API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetExecutionHistory:
    get:
      summary: Get Execution History
      description: Returns the history of the specified execution as a list of events.
      operationId: getExecutionHistory
      x-api-path-slug: actiongetexecutionhistory-get
      parameters:
      - in: query
        name: executionArn
        description: The Amazon Resource Name (ARN) of the execution
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results that will be returned per call
        type: string
      - in: query
        name: nextToken
        description: If a nextToken was returned by a previous call, there are more
          results available
        type: string
      - in: query
        name: reverseOrder
        description: Lists events in descending order of their timeStamp
        type: string
      responses:
        200:
          description: OK
      tags:
      - Execution