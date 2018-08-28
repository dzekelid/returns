---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Get Inventory Schema
  version: 1.0.0
  description: |-
    Return a list of inventory type names for the account, or return a list of attribute
       names for a specific Inventory item type.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribePatchGroupState:
    get:
      summary: Describe Patch Group State
      description: Returns high-level aggregated patch compliance state for a patch
        group.
      operationId: describePatchGroupState
      x-api-path-slug: actiondescribepatchgroupstate-get
      parameters:
      - in: query
        name: PatchGroup
        description: The name of the patch group whose patch snapshot should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - State
  /?Action=GetCommandInvocation:
    get:
      summary: Get Command Invocation
      description: Returns detailed information about command execution for an invocation
        or plugin.
      operationId: getCommandInvocation
      x-api-path-slug: actiongetcommandinvocation-get
      parameters:
      - in: query
        name: CommandId
        description: (Required) The parent command ID of the invocation plugin
        type: string
      - in: query
        name: InstanceId
        description: (Required) The ID of the managed instance targeted by the command
        type: string
      - in: query
        name: PluginName
        description: (Optional) The name of the plugin for which you want detailed
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Command
      - Invocation
  /?Action=GetInventorySchema:
    get:
      summary: Get Inventory Schema
      description: |-
        Return a list of inventory type names for the account, or return a list of attribute
           names for a specific Inventory item type.
      operationId: getInventorySchema
      x-api-path-slug: actiongetinventoryschema-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TypeName
        description: The type of inventory item to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
      - Schema
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