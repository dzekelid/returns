---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Get Appliances
  description: Returns an appliance based on its ID.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get Account
      description: Returns the global account information. **Not implemented**
      operationId: GetAccount
      x-api-path-slug: account-get
      parameters:
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Account
  /appliances:
    get:
      summary: Get Appliances
      description: Returns appliances.
      operationId: GetAppliance
      x-api-path-slug: appliances-get
      parameters:
      - in: query
        name: name
        description: The name of the desired appliance
      - in: query
        name: regionUri
        description: Set of appliances in this region
      responses:
        200:
          description: OK
      tags:
      - Appliances
  /appliances/{id}:
    get:
      summary: Get Appliances
      description: Returns an appliance based on its ID.
      operationId: GetApplianceById
      x-api-path-slug: appliancesid-get
      parameters:
      - in: path
        name: id
        description: ID of the appliance to retrieve
      responses:
        200:
          description: OK
      tags:
      - Appliances
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