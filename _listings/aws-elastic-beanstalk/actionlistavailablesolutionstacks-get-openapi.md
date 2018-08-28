---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 0
info:
  title: AWS Elastic Beanstalk API List Available Solution Stacks
  version: 1.0.0
  description: Returns a list of the available solution stack names.
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
  /?Action=DescribeConfigurationSettings:
    get:
      summary: Describe Configuration Settings
      description: |-
        Returns a description of the settings for the specified configuration set, that is,
              either a configuration template or the configuration set associated with a running
              environment.
      operationId: describeConfigurationSettings
      x-api-path-slug: actiondescribeconfigurationsettings-get
      parameters:
      - in: query
        name: ApplicationName
        description: The application for the environment or configuration template
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to describe
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Settings
  /?Action=DescribeEnvironmentHealth:
    get:
      summary: Describe Environment Health
      description: Returns information about the overall health of the specified environment.
      operationId: describeEnvironmentHealth
      x-api-path-slug: actiondescribeenvironmenthealth-get
      parameters:
      - in: query
        name: AttributeNames.member.N
        description: Specify the response elements to return
        type: string
      - in: query
        name: EnvironmentId
        description: Specify the environment by ID
        type: string
      - in: query
        name: EnvironmentName
        description: Specify the environment by name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEnvironmentResources:
    get:
      summary: Describe Environment Resources
      description: Returns AWS resources for this environment.
      operationId: describeEnvironmentResources
      x-api-path-slug: actiondescribeenvironmentresources-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to retrieve AWS resource usage data
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to retrieve AWS resource usage data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEnvironments:
    get:
      summary: Describe Environments
      description: Returns descriptions for existing environments.
      operationId: describeEnvironments
      x-api-path-slug: actiondescribeenvironments-get
      parameters:
      - in: query
        name: ApplicationName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that are associated with this application
        type: string
      - in: query
        name: EnvironmentIds.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that have the specified IDs
        type: string
      - in: query
        name: EnvironmentNames.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that have the specified names
        type: string
      - in: query
        name: IncludedDeletedBackTo
        description: If specified when IncludeDeleted is set to true, then      environments
          deleted after this date are displayed
        type: string
      - in: query
        name: IncludeDeleted
        description: 'Indicates whether to include deleted environments:'
        type: string
      - in: query
        name: VersionLabel
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that are associated with this application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEvents:
    get:
      summary: Describe Events
      description: Returns list of event descriptions matching criteria up to the
        last 6 weeks.
      operationId: describeEvents
      x-api-path-slug: actiondescribeevents-get
      parameters:
      - in: query
        name: ApplicationName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those associated with this application
        type: string
      - in: query
        name: EndTime
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      occur up to, but not including, the EndTime
        type: string
      - in: query
        name: EnvironmentId
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this environment
        type: string
      - in: query
        name: EnvironmentName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this environment
        type: string
      - in: query
        name: MaxRecords
        description: Specifies the maximum number of events that can be returned,
          beginning with the most      recent event
        type: string
      - in: query
        name: NextToken
        description: Pagination token
        type: string
      - in: query
        name: RequestId
        description: If specified, AWS Elastic Beanstalk restricts the described events
          to include only      those associated with this request ID
        type: string
      - in: query
        name: Severity
        description: If specified, limits the events returned from this call to include
          only those with the      specified severity or higher
        type: string
      - in: query
        name: StartTime
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      occur on or after this time
        type: string
      - in: query
        name: TemplateName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      are associated with this environment configuration
        type: string
      - in: query
        name: VersionLabel
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=ListAvailableSolutionStacks:
    get:
      summary: List Available Solution Stacks
      description: Returns a list of the available solution stack names.
      operationId: listAvailableSolutionStacks
      x-api-path-slug: actionlistavailablesolutionstacks-get
      parameters:
      - in: query
        name: SolutionStackDetails.member.N
        description: A list of available solution stacks and their SolutionStackDescription
        type: string
      - in: query
        name: SolutionStacks.member.N
        description: A list of available solution stacks
        type: string
      responses:
        200:
          description: OK
      tags:
      - Solution Stacks
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