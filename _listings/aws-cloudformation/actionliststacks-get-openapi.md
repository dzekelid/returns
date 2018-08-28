---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 0
info:
  title: AWS CloudFormation API List Stacks
  version: 1.0.0
  description: Returns the summary information for stacks whose status matches the
    specified StackStatusFilter.
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
  /?Action=GetStackPolicy:
    get:
      summary: Get Stack Policy
      description: Returns the stack policy for a specified stack.
      operationId: getStackPolicy
      x-api-path-slug: actiongetstackpolicy-get
      parameters:
      - in: query
        name: StackName
        description: The name or unique stack ID that is associated with the stack
          whose policy you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Policies
  /?Action=GetTemplate:
    get:
      summary: Get Template
      description: Returns the template body for a specified stack.
      operationId: getTemplate
      x-api-path-slug: actiongettemplate-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of a change set for which
          AWS CloudFormation returns the associated template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      - in: query
        name: TemplateStage
        description: For templates that include transforms, the stage of the template
          that AWS CloudFormation returns
        type: string
      responses:
        200:
          description: OK
      tags:
      - Templates
  /?Action=GetTemplateSummary:
    get:
      summary: Get Template Summary
      description: Returns information about a new or existing template.
      operationId: getTemplateSummary
      x-api-path-slug: actiongettemplatesummary-get
      parameters:
      - in: query
        name: StackName
        description: The name or the stack ID that is associated with the stack, which
          are not always interchangeable
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
      - Templates
  /?Action=ListChangeSets:
    get:
      summary: List Change Sets
      description: Returns the ID and status of each active change set for a stack.
      operationId: listChangeSets
      x-api-path-slug: actionlistchangesets-get
      parameters:
      - in: query
        name: NextToken
        description: A string (provided by the ListChangeSets response output) that
          identifies the next page of change sets that you want to retrieve
        type: string
      - in: query
        name: StackName
        description: The name or the Amazon Resource Name (ARN) of the stack for which
          you want to list change sets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=ListStackResources:
    get:
      summary: List Stack Resources
      description: Returns descriptions of all resources of the specified stack.
      operationId: listStackResources
      x-api-path-slug: actionliststackresources-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stack resources that
          you want to retrieve
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
  /?Action=ListStacks:
    get:
      summary: List Stacks
      description: Returns the summary information for stacks whose status matches
        the specified StackStatusFilter.
      operationId: listStacks
      x-api-path-slug: actionliststacks-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stacks that you want
          to retrieve
        type: string
      - in: query
        name: StackStatusFilter.member.N
        description: Stack status to use as a filter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
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