swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?cors:
    get:
      summary: GET Bucket CORS
      description: Returns the cors configuration information set for thebucket
      operationId: get-bucket-cors
      x-api-path-slug: cors-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - CORS
  /?replication:
    get:
      summary: GET Bucket replication
      description: Returns the replication configuration information set on the      bucket
      operationId: get-bucket-replication
      x-api-path-slug: replication-get
      parameters:
      - in: query
        name: AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo;
          API Reference &raquo; Operations on Buckets &raquo; GET Bucket replication
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Replication