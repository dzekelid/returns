---
swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 0
info:
  title: AWS WAF API Get Change Token Status
  version: 1.0.0
  description: 'Service: AWS WAFReturns the status of a ChangeToken that you got by
    calling.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetByteMatchSet:
    get:
      summary: Get Byte Match Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getByteMatchSet
      x-api-path-slug: actiongetbytematchset-get
      parameters:
      - in: query
        name: ByteMatchSetId
        description: The ByteMatchSetId of the ByteMatchSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Set
  /?Action=GetChangeTokenStatus:
    get:
      summary: Get Change Token Status
      description: 'Service: AWS WAFReturns the status of a ChangeToken that you got
        by calling.'
      operationId: getChangeTokenStatus
      x-api-path-slug: actiongetchangetokenstatus-get
      parameters:
      - in: query
        name: ChangeToken
        description: The change token for which you want to get the status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Token
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