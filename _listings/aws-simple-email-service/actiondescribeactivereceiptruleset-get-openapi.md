---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Describe Active Receipt Rule Set
  version: 1.0.0
  description: Returns the metadata and receipt rules for the receipt rule set that
    is currently active.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeActiveReceiptRuleSet:
    get:
      summary: Describe Active Receipt Rule Set
      description: Returns the metadata and receipt rules for the receipt rule set
        that is currently active.
      operationId: describeActiveReceiptRuleSet
      x-api-path-slug: actiondescribeactivereceiptruleset-get
      parameters:
      - in: query
        name: Metadata
        description: The metadata for the currently active receipt rule set
        type: string
      - in: query
        name: Rules.member.N
        description: The receipt rules that belong to the active rule set
        type: string
      responses:
        200:
          description: OK
      tags:
      - Receipt Rule Sets
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