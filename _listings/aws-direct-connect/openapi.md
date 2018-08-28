swagger: "2.0"
x-collection-name: AWS Direct Connect
x-complete: 1
info:
  title: AWS Direct Connect API
  version: 1.0.0
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
  /?Action=DescribeInterconnectLoa:
    get:
      summary: Describe Interconnect Loa
      description: Returns the LOA-CFA for an Interconnect.
      operationId: describeInterconnectLoa
      x-api-path-slug: actiondescribeinterconnectloa-get
      parameters:
      - in: query
        name: interconnectId
        description: The ID of the interconnect
        type: string
      - in: query
        name: loaContentType
        description: A standard media type indicating the content type of the LOA-CFA
          document
        type: string
      - in: query
        name: providerName
        description: The name of the service provider who establishes connectivity
          on your behalf
        type: string
      responses:
        200:
          description: OK
      tags:
      - Interconnects
  /?Action=DescribeInterconnects:
    get:
      summary: Describe Interconnects
      description: Returns a list of interconnects owned by the AWS account.
      operationId: describeInterconnects
      x-api-path-slug: actiondescribeinterconnects-get
      parameters:
      - in: query
        name: interconnectId
        description: The ID of the interconnect
        type: string
      responses:
        200:
          description: OK
      tags:
      - Interconnects
  /?Action=DescribeLocations:
    get:
      summary: Describe Locations
      description: Returns the list of AWS Direct Connect locations in the current
        AWS region.
      operationId: describeLocations
      x-api-path-slug: actiondescribelocations-get
      parameters:
      - in: query
        name: locations
        description: A list of colocation hubs where network providers have equipment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Locations
  /?Action=DescribeVirtualGateways:
    get:
      summary: Describe Virtual Gateways
      description: Returns a list of virtual private gateways owned by the AWS account.
      operationId: describeVirtualGateways
      x-api-path-slug: actiondescribevirtualgateways-get
      parameters:
      - in: query
        name: virtualGateways
        description: A list of virtual private gateways
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual Gateways