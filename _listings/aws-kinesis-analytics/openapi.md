swagger: "2.0"
x-collection-name: AWS Kinesis Analytics
x-complete: 1
info:
  title: AWS Kinesis Analytics API
  version: 1.0.0
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