---
swagger: "2.0"
x-collection-name: Strava
x-complete: 0
info:
  title: Strava List Activity Comments
  description: Returns the comments on the given activity.
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities/{id}:
    get:
      summary: Get Activity
      description: Returns the given activity that is owned by the authenticated athlete.
      operationId: getActivityById
      x-api-path-slug: activitiesid-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      - in: query
        name: include_all_efforts
        description: To include all segments efforts
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Activity
  /activities/{id}/comments:
    get:
      summary: List Activity Comments
      description: Returns the comments on the given activity.
      operationId: getCommentsByActivityId
      x-api-path-slug: activitiesidcomments-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Activity
      - Comments
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