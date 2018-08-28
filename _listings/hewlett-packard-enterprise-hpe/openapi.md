swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
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