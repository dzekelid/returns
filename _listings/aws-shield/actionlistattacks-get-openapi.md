---
swagger: "2.0"
x-collection-name: AWS Shield
x-complete: 0
info:
  title: AWS Shield API List Attacks
  version: 1.0.0
  description: |-
    Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
             period.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAttacks:
    get:
      summary: List Attacks
      description: |-
        Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
                 period.
      operationId: listAttacks
      x-api-path-slug: actionlistattacks-get
      parameters:
      - in: query
        name: EndTime
        description: The end of the time period for the attacks
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of AttackSummary objects to be returned
        type: string
      - in: query
        name: NextToken
        description: The ListAttacksRequest
        type: string
      - in: query
        name: ResourceArns
        description: The ARN (Amazon Resource Name) of the resource that was attacked
        type: string
      - in: query
        name: StartTime
        description: The time period for the attacks
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attacks
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