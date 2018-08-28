---
swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 0
info:
  title: HealthCare.gov Get Topics
  version: 1.0.0
  description: Returns pages content.
host: www.healthcare.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/articles{mediaTypeExtension}:
    get:
      summary: Get Articles
      description: Returns pages content.
      operationId: getApiArticlesMediatypeextension
      x-api-path-slug: apiarticlesmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Articles
  /api/blog{mediaTypeExtension}:
    get:
      summary: Get Blog
      description: Returns pages content.
      operationId: getApiBlogMediatypeextension
      x-api-path-slug: apiblogmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Blog
  /api/glossary{mediaTypeExtension}:
    get:
      summary: Get Glossary
      description: Returns pages content.
      operationId: getApiGlossaryMediatypeextension
      x-api-path-slug: apiglossarymediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Glossary
  /api/questions{mediaTypeExtension}:
    get:
      summary: Get Questions
      description: Returns pages content.
      operationId: getApiQuestionsMediatypeextension
      x-api-path-slug: apiquestionsmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Questions
  /api/states{mediaTypeExtension}:
    get:
      summary: Get States
      description: Returns pages content.
      operationId: getApiStatesMediatypeextension
      x-api-path-slug: apistatesmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - States
  /api/topics{mediaTypeExtension}:
    get:
      summary: Get Topics
      description: Returns pages content.
      operationId: getApiTopicsMediatypeextension
      x-api-path-slug: apitopicsmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Topics
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