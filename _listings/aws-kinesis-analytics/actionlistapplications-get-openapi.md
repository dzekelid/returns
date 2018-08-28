---
swagger: "2.0"
x-collection-name: AWS Kinesis Analytics
x-complete: 0
info:
  title: AWS Kinesis Analytics API List Applications
  version: 1.0.0
  description: Returns a list of Amazon Kinesis Analytics applications in your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeApplication:
    get:
      summary: Describe Application
      description: Returns information about a specific Amazon Kinesis Analytics application.
      operationId: describeApplication
      x-api-path-slug: actiondescribeapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=ListApplications:
    get:
      summary: List Applications
      description: Returns a list of Amazon Kinesis Analytics applications in your
        account.
      operationId: listApplications
      x-api-path-slug: actionlistapplications-get
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