---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Return a collect with a certain id
  description: Return a collect with a certain id.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/collects/20713233987.json:
    get:
      summary: Return a collect with a certain id
      description: Return a collect with a certain id.
      operationId: getAdminCollects20713233987.json
      x-api-path-slug: admincollects20713233987-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Return
      - Collect
      - Certain
      - Id
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