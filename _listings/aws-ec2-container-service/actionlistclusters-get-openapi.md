---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API List Clusters
  version: 1.0.0
  description: Returns a list of existing clusters.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Returns a list of existing clusters.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of cluster results returned by ListClusters
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListClusters
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
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