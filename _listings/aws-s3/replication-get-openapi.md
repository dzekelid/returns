---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 GET Bucket replication
  version: 1.0.0
  description: Returns the replication configuration information set on the      bucket
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