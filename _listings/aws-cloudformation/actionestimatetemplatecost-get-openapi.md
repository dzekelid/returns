---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 0
info:
  title: AWS CloudFormation API Estimate Template Cost
  version: 1.0.0
  description: Returns the estimated monthly cost of a template.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeChangeSet:
    get:
      summary: Describe Change Set
      description: Returns the inputs for the change set and a list of changes that
        AWS CloudFormation will make if you execute the change set.
      operationId: describeChangeSet
      x-api-path-slug: actiondescribechangeset-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of the change set that
          you want to describe
        type: string
      - in: query
        name: NextToken
        description: A string (provided by the DescribeChangeSet response output)
          that identifies the next page of information that you want to retrieve
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set, specify the stack
          name or ID (ARN) of the change set you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=DescribeStackEvents:
    get:
      summary: Describe Stack Events
      description: Returns all stack related events for a specified stack in reverse
        chronological order.
      operationId: describeStackEvents
      x-api-path-slug: actiondescribestackevents-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of events that you want
          to retrieve
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Events
  /?Action=DescribeStackResource:
    get:
      summary: Describe Stack Resource
      description: Returns a description of the specified resource in the specified
        stack.
      operationId: describeStackResource
      x-api-path-slug: actiondescribestackresource-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical name of the resource as specified in the template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=DescribeStackResources:
    get:
      summary: Describe Stack Resources
      description: Returns AWS resource descriptions for running and deleted stacks.
      operationId: describeStackResources
      x-api-path-slug: actiondescribestackresources-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical name of the resource as specified in the template
        type: string
      - in: query
        name: PhysicalResourceId
        description: The name or unique identifier that corresponds to a physical
          instance ID of a resource supported by AWS CloudFormation
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=DescribeStacks:
    get:
      summary: Describe Stacks
      description: Returns the description for the specified stack; if no stack name
        was specified, then it returns the description for all the stacks created.
      operationId: describeStacks
      x-api-path-slug: actiondescribestacks-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stacks that you want
          to retrieve
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=EstimateTemplateCost:
    get:
      summary: Estimate Template Cost
      description: Returns the estimated monthly cost of a template.
      operationId: estimateTemplateCost
      x-api-path-slug: actionestimatetemplatecost-get
      parameters:
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      responses:
        200:
          description: OK
      tags:
      - Template Cost
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