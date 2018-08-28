---
swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 0
info:
  title: AWS WAF API Get Byte Match Set
  version: 1.0.0
  description: 'Service: AWS WAFReturns the.'
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