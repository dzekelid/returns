swagger: "2.0"
x-collection-name: AWS Rekognition
x-complete: 1
info:
  title: AWS Rekognition API
  version: 1.0.0
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