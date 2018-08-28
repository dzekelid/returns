swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEndpoints:
    get:
      summary: Describe Endpoints
      description: Returns information about the endpoints for your account in the
        current region.
      operationId: describeEndpoints
      x-api-path-slug: actiondescribeendpoints-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=DescribeEndpointTypes:
    get:
      summary: Describe Endpoint Types
      description: Returns information about the type of endpoints available.
      operationId: describeEndpointTypes
      x-api-path-slug: actiondescribeendpointtypes-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoint Types
  /?Action=DescribeOrderableReplicationInstances:
    get:
      summary: Describe Orderable Replication Instances
      description: Returns information about the replication instance types that can
        be created in the specified region.
      operationId: describeOrderableReplicationInstances
      x-api-path-slug: actiondescribeorderablereplicationinstances-get
      parameters:
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DescribeRefreshSchemasStatus:
    get:
      summary: Describe Refresh Schemas Status
      description: Returns the status of the RefreshSchemas operation.
      operationId: describeRefreshSchemasStatus
      x-api-path-slug: actiondescriberefreshschemasstatus-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schemas
  /?Action=DescribeReplicationInstances:
    get:
      summary: Describe Replication Instances
      description: Returns information about replication instances for your account
        in the current region.
      operationId: describeReplicationInstances
      x-api-path-slug: actiondescribereplicationinstances-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DescribeReplicationSubnetGroups:
    get:
      summary: Describe Replication Subnet Groups
      description: Returns information about the replication subnet groups.
      operationId: describeReplicationSubnetGroups
      x-api-path-slug: actiondescribereplicationsubnetgroups-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DescribeReplicationTasks:
    get:
      summary: Describe Replication Tasks
      description: Returns information about replication tasks for your account in
        the current region.
      operationId: describeReplicationTasks
      x-api-path-slug: actiondescribereplicationtasks-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous     request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=DescribeSchemas:
    get:
      summary: Describe Schemas
      description: Returns information about the schema for the specified endpoint.
      operationId: describeSchemas
      x-api-path-slug: actiondescribeschemas-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous     request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schemas
  /?Action=DescribeTableStatistics:
    get:
      summary: Describe Table Statistics
      description: Returns table statistics on the database migration task, including
        table name, rows inserted, rows updated, and rows deleted.
      operationId: describeTableStatistics
      x-api-path-slug: actiondescribetablestatistics-get
      parameters:
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Name (ARN) of the replication task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Table Statistics