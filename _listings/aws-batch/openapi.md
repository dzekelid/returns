swagger: "2.0"
x-collection-name: AWS Batch
x-complete: 1
info:
  title: AWS Batch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListJobs:
    get:
      summary: List Jobs
      description: Returns a list of task jobs for a specified job queue.
      operationId: listJobs
      x-api-path-slug: actionlistjobs-get
      parameters:
      - in: query
        name: jobQueue
        description: The name or full Amazon Resource Name (ARN) of the job queue
          with which to list jobs
        type: string
      - in: query
        name: jobStatus
        description: The job status with which to filter jobs in the specified queue
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results returned by ListJobs in paginated
          output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated            ListJobs
          request where maxResults was used and the results         exceeded the value
          of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs