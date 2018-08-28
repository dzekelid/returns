---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: Victor Ops A list of shift changes for a team
  description: |-
    Returns a log of user shift changes for the specified team. This is historical
    data, and may be up to 15 minutes behind real-time log data.

    This API may be called a maximum of 6 times per minute.
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-reporting/v1/team/{team}/oncall/log:
    get:
      summary: A list of shift changes for a team
      description: |-
        Returns a log of user shift changes for the specified team. This is historical
        data, and may be up to 15 minutes behind real-time log data.

        This API may be called a maximum of 6 times per minute.
      operationId: api_reporting.v1.team.team.oncall.log.get
      x-api-path-slug: apireportingv1teamteamoncalllog-get
      parameters:
      - in: query
        name: end
        description: Return shift changes occurring before this timestamp
      - in: query
        name: No Name
      - in: query
        name: start
        description: Return shift changes occurring after this timestamp
      - in: path
        name: team
        description: The VictorOps team slug
      - in: query
        name: userName
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Api-reporting
      - V1
      - Team
      - Team
      - Oncall
      - Log
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