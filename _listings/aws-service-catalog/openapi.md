swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 1
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListLaunchPaths:
    get:
      summary: List Launch Paths
      description: Returns a paginated list of all paths to a specified product.
      operationId: listLaunchPaths
      x-api-path-slug: actionlistlaunchpaths-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Launch Paths
  /?Action=ListRecordHistory:
    get:
      summary: List Record History
      description: |-
        Returns a paginated list of all performed requests, in the form of RecordDetails
                 objects that are filtered as specified.
      operationId: listRecordHistory
      x-api-path-slug: actionlistrecordhistory-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccessLevelFilter
        description: The access level for obtaining results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: SearchFilter
        description: The filter to limit search results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Record History
  /?Action=ScanProvisionedProducts:
    get:
      summary: Scan Provisioned Products
      description: |-
        Returns a paginated list of all the ProvisionedProduct objects that are currently
                 available (not terminated).
      operationId: scanProvisionedProducts
      x-api-path-slug: actionscanprovisionedproducts-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccessLevelFilter
        description: The access level for obtaining results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioned Products
  /?Action=SearchProducts:
    get:
      summary: Search Products
      description: |-
        Returns a paginated list all of the Products objects to which the caller
                 has access.
      operationId: searchProducts
      x-api-path-slug: actionsearchproducts-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Filters
        description: The list of filters with which to limit search results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: SortBy
        description: The sort field specifier
        type: string
      - in: query
        name: SortOrder
        description: The sort order specifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products