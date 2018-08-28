swagger: "2.0"
x-collection-name: AWS Shield
x-complete: 1
info:
  title: AWS Shield API
  version: 1.0.0
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