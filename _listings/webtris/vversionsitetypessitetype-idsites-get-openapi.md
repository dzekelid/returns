---
swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 0
info:
  title: WebTRIS Traffic Flow API Returns the layer metadata for the LayerId specified.
  version: 1.0.0
  description: Returns the layer metadata for the layerid specified..
host: webtris.highwaysengland.co.uk
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v{version}/areas:
    get:
      summary: Returns list of areas
      description: Returns list of areas.
      operationId: Areas_Get
      x-api-path-slug: vversionareas-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Areas
  /v{version}/areas/{area_Ids}:
    get:
      summary: Returns details of selected area
      description: Returns details of selected area.
      operationId: Areas_Get
      x-api-path-slug: vversionareasarea-ids-get
      parameters:
      - in: path
        name: area_Ids
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Details
      - Of
      - Selected
      - Area
  /v{version}/sitetypes/{siteType_Id}/sites:
    get:
      summary: Returns the layer metadata for the LayerId specified.
      description: Returns the layer metadata for the layerid specified..
      operationId: SiteTypes_GetSitesForPublicFacingAPI
      x-api-path-slug: vversionsitetypessitetype-idsites-get
      parameters:
      - in: path
        name: siteType_Id
        description: 1 = MIDAS, 2 = TAME, 3 = TMU, 4 = TRADS Legacy
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Layer
      - Metadatathe
      - LayerId
      - Specified
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