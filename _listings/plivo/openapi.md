swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Plivo
  version: 1.0.0
host: api.plivo.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/{id}/resources:
    get:
      summary: Get Account Resources
      description: 'Returns used resources, provided by subscriptions. Roles: account/owner,
        account/member, system/manager, system/admin.'
      operationId: getResources
      x-api-path-slug: accountidresources-get
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: query
        name: serviceId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Resources