---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 0
info:
  title: AWS Elastic Beanstalk API Describe Applications
  version: 1.0.0
  description: Returns the descriptions of existing applications.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeApplications:
    get:
      summary: Describe Applications
      description: Returns the descriptions of existing applications.
      operationId: describeApplications
      x-api-path-slug: actiondescribeapplications-get
      parameters:
      - in: query
        name: ApplicationNames.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to only include      those with the specified names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
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