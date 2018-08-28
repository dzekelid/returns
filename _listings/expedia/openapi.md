swagger: "2.0"
x-collection-name: Expedia
x-complete: 1
info:
  title: Expedia
  description: expedia-mobile-api-documentation--brfont-colorblue-note-in-case-of-authorization-exception-just-a-hrefstaticmobileswaggeruiusersigninusersigninafont
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/users/{userId}/trips:
    get:
      summary: (Internal Only)
      description: (Internal Only) Returns array of trips for passed userId
      operationId: trips-by-user-id
      x-api-path-slug: apiusersuseridtrips-get
      parameters:
      - in: path
        name: userId
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Users