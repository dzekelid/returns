---
swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 0
info:
  title: Azure Blockchain Workbench Get Api Health
  description: |-
    Returns the health of the system. See https://docs.microsoft.com/en-us/azure/architecture/patterns/health-endpoint-monitoring
                 for more details.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/health:
    get:
      summary: Get Api Health
      description: |-
        Returns the health of the system. See https://docs.microsoft.com/en-us/azure/architecture/patterns/health-endpoint-monitoring
                     for more details.
      operationId: Health
      x-api-path-slug: apihealth-get
      responses:
        200:
          description: OK
      tags:
      - Api
      - Health
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