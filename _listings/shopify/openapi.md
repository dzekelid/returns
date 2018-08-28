swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
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