swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 1
info:
  title: AWS Code Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcknowledgeJob:
    get:
      summary: Acknowledge Job
      description: |-
        Returns information about a specified job and whether that job has been received by
                    the job worker.
      operationId: acknowledgeJob
      x-api-path-slug: actionacknowledgejob-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job for which you want
          to confirm            receipt
        type: string
      - in: query
        name: nonce
        description: A system-generated random number that AWS CodePipeline uses to
          ensure that the job            is being worked on by only one job worker
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the EBS snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Job
  /?Action=GetJobDetails:
    get:
      summary: Get Job Details
      description: Returns information about a job.
      operationId: getJobDetails
      x-api-path-slug: actiongetjobdetails-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID for the job
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job
      - Details
  /?Action=GetPipeline:
    get:
      summary: Get Pipeline
      description: Returns the metadata, structure, stages, and actions of a pipeline.
      operationId: getPipeline
      x-api-path-slug: actiongetpipeline-get
      parameters:
      - in: query
        name: Attribute
        description: The snapshot attribute to modify
        type: string
      - in: query
        name: CreateVolumePermission
        description: A JSON representation of the snapshot attribute modification
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline for which you want to get information
        type: string
      - in: query
        name: OperationType
        description: The type of operation to perform to the attribute
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      - in: query
        name: UserGroup.N
        description: The group to modify for the snapshot
        type: string
      - in: query
        name: UserId.N
        description: The account ID to modify for the snapshot
        type: string
      - in: query
        name: version
        description: The version number of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=GetPipelineExecution:
    get:
      summary: Get Pipeline Execution
      description: |-
        Returns information about an execution of a pipeline, including details about
                    artifacts, the pipeline execution ID, and the name, version, and status of the
                    pipeline.
      operationId: getPipelineExecution
      x-api-path-slug: actiongetpipelineexecution-get
      parameters:
      - in: query
        name: AutoEnableIO
        description: Indicates whether the volume should be auto-enabled for I/O operations
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: pipelineExecutionId
        description: The ID of the pipeline execution about which you want to get
          execution            details
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline about which you want to get execution
          details
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
      - Execution
  /?Action=GetPipelineState:
    get:
      summary: Get Pipeline State
      description: |-
        Returns information about the state of a pipeline, including the stages and
                    actions.
      operationId: getPipelineState
      x-api-path-slug: actiongetpipelinestate-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline about which you want to get information
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
      - State
  /?Action=PollForJobs:
    get:
      summary: Poll For Jobs
      description: Returns information about any jobs for AWS CodePipeline to act
        upon.
      operationId: pollForJobs
      x-api-path-slug: actionpollforjobs-get
      parameters:
      - in: query
        name: actionTypeId
        description: Represents information about an action type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: maxBatchSize
        description: The maximum number of jobs to return in a poll for jobs call
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      - in: query
        name: PublicIp.N
        description: One or more Elastic IP addresses
        type: string
      - in: query
        name: queryParam
        description: A map of property names and values
        type: string
      responses:
        200:
          description: OK
      tags:
      - PollJobs