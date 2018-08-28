swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 1
info:
  title: ""
  version: 1.0.0
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
  /v{version}/sitetypes:
    get:
      summary: Return list of site types
      description: Return list of site types.
      operationId: SiteTypes_Index
      x-api-path-slug: vversionsitetypes-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Site
      - Types