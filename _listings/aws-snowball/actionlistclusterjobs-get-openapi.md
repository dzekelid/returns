---
swagger: "2.0"
x-collection-name: AWS Snowball
x-complete: 0
info:
  title: AWS Snowball API List Cluster Jobs
  version: 1.0.0
  description: Returns an array of JobListEntry objects of the specified length.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAddresses:
    get:
      summary: Describe Addresses
      description: Returns a specified number of ADDRESS objects.
      operationId: describeAddresses
      x-api-path-slug: actiondescribeaddresses-get
      parameters:
      - in: query
        name: MaxResults
        description: The number of ADDRESS objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Addresses
  /?Action=DescribeCluster:
    get:
      summary: Describe Cluster
      description: |-
        Returns information about a specific cluster including shipping information, cluster
              status, and other important metadata.
      operationId: describeCluster
      x-api-path-slug: actiondescribecluster-get
      parameters:
      - in: query
        name: ClusterId
        description: The automatically generated ID for a cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeJob:
    get:
      summary: Describe Job
      description: |-
        Returns information about a specific job including shipping information, job status,
              and other important metadata.
      operationId: describeJob
      x-api-path-slug: actiondescribejob-get
      parameters:
      - in: query
        name: JobId
        description: The automatically generated ID for a job, for example        JID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=GetJobManifest:
    get:
      summary: Get Job Manifest
      description: |-
        Returns a link to an Amazon S3 presigned URL for the manifest file associated with the
              specified JobId value.
      operationId: getJobManifest
      x-api-path-slug: actiongetjobmanifest-get
      parameters:
      - in: query
        name: JobId
        description: The ID for a job that you want to get the manifest file for,
          for example        JID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Manifest
  /?Action=GetJobUnlockCode:
    get:
      summary: Get Job Unlock Code
      description: Returns the UnlockCode code value for the specified job.
      operationId: getJobUnlockCode
      x-api-path-slug: actiongetjobunlockcode-get
      parameters:
      - in: query
        name: JobId
        description: The ID for the job that you want to get the UnlockCode value
          for, for      example JID123e4567-e89b-12d3-a456-426655440000
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=GetSnowballUsage:
    get:
      summary: Get Snowball Usage
      description: |-
        Returns information about the Snowball service limit for your account, and also the
              number of Snowballs your account has in use.
      operationId: getSnowballUsage
      x-api-path-slug: actiongetsnowballusage-get
      parameters:
      - in: query
        name: SnowballLimit
        description: The service limit for number of Snowballs this account can have
          at once
        type: string
      - in: query
        name: SnowballsInUse
        description: The number of Snowballs that this account is currently using
        type: string
      responses:
        200:
          description: OK
      tags:
      - Usage
  /?Action=ListClusterJobs:
    get:
      summary: List Cluster Jobs
      description: Returns an array of JobListEntry objects of the specified length.
      operationId: listClusterJobs
      x-api-path-slug: actionlistclusterjobs-get
      parameters:
      - in: query
        name: ClusterId
        description: The 39-character ID for the cluster that you want to list, for
          example        CID123e4567-e89b-12d3-a456-426655440000
        type: string
      - in: query
        name: MaxResults
        description: The number of JobListEntry objects to return
        type: string
      - in: query
        name: NextToken
        description: HTTP requests are stateless
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Jobs
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