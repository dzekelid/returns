---
swagger: "2.0"
x-collection-name: AWS Rekognition
x-complete: 0
info:
  title: AWS Rekognition API List Faces
  version: 1.0.0
  description: Returns metadata for faces in the specified collection.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListCollections:
    get:
      summary: List Collections
      description: Returns list of collection IDs in your account.
      operationId: listCollections
      x-api-path-slug: actionlistcollections-get
      parameters:
      - in: query
        name: MaxResults
        description: Maximum number of collection IDs to return
        type: string
      - in: query
        name: NextToken
        description: Pagination token from the previous response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections
  /?Action=ListFaces:
    get:
      summary: List Faces
      description: Returns metadata for faces in the specified collection.
      operationId: listFaces
      x-api-path-slug: actionlistfaces-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection from which to list the faces
        type: string
      - in: query
        name: MaxResults
        description: Maximum number of faces to return
        type: string
      - in: query
        name: NextToken
        description: If the previous response was incomplete (because there is more
          data to retrieve), Amazon Rekognition      returns a pagination token in
          the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
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