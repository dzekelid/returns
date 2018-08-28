---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 0
info:
  title: AWS Elastic Beanstalk API Describe Configuration Settings
  version: 1.0.0
  description: |-
    Returns a description of the settings for the specified configuration set, that is,
          either a configuration template or the configuration set associated with a running
          environment.
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