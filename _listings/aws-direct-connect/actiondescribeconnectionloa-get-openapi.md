---
swagger: "2.0"
x-collection-name: AWS Direct Connect
x-complete: 0
info:
  title: AWS Direct Connect API Describe Connection Loa
  version: 1.0.0
  description: Returns the LOA-CFA for a Connection.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeConnectionLoa:
    get:
      summary: Describe Connection Loa
      description: Returns the LOA-CFA for a Connection.
      operationId: describeConnectionLoa
      x-api-path-slug: actiondescribeconnectionloa-get
      parameters:
      - in: query
        name: connectionId
        description: ID of the connection
        type: string
      - in: query
        name: loaContentType
        description: A standard media type indicating the content type of the LOA-CFA
          document
        type: string
      - in: query
        name: providerName
        description: The name of the APN partner or service provider who establishes
          connectivity on your behalf
        type: string
      responses:
        200:
          description: OK
      tags:
      - Connections
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