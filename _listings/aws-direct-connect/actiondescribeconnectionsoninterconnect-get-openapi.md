---
swagger: "2.0"
x-collection-name: AWS Direct Connect
x-complete: 0
info:
  title: AWS Direct Connect API Describe Connections On Interconnect
  version: 1.0.0
  description: Return a list of connections that have been provisioned on the given
    interconnect.
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
  /?Action=DescribeConnectionsOnInterconnect:
    get:
      summary: Describe Connections On Interconnect
      description: Return a list of connections that have been provisioned on the
        given interconnect.
      operationId: describeConnectionsOnInterconnect
      x-api-path-slug: actiondescribeconnectionsoninterconnect-get
      parameters:
      - in: query
        name: interconnectId
        description: ID of the interconnect on which a list of connection is provisioned
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