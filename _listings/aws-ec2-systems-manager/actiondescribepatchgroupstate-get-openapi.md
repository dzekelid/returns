---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Describe Patch Group State
  version: 1.0.0
  description: Returns high-level aggregated patch compliance state for a patch group.
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