---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Get Rate Limit Sttaus
  description: Returns the current rate limits for methods belonging to the specified
    resource families
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /application/rate_limit_status:
    get:
      summary: Get Rate Limit Sttaus
      description: Returns the current rate limits for methods belonging to the specified
        resource families
      operationId: returns-the-current-rate-limits-for-methods-belonging-to-the-specified-resource-families
      x-api-path-slug: applicationrate-limit-status-get
      parameters:
      - in: query
        name: resources
        description: A comma-separated list of resource families you want to know
          the current rate limit disposition for
      responses:
        200:
          description: OK
      tags:
      - Rate Limit
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