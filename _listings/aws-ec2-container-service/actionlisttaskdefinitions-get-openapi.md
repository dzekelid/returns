---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API List Task Definitions
  version: 1.0.0
  description: Returns a list of task definitions that are registered to your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Returns a list of existing clusters.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of cluster results returned by ListClusters
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListClusters
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ListContainerInstances:
    get:
      summary: List Container Instances
      description: Returns a list of container instances in a specified cluster.
      operationId: listContainerInstances
      x-api-path-slug: actionlistcontainerinstances-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instances            to list
        type: string
      - in: query
        name: filter
        description: You can filter the results of a ListContainerInstances operation
          with            cluster query language statements
        type: string
      - in: query
        name: maxResults
        description: The maximum number of container instance results returned by                ListContainerInstances
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListContainerInstances
          request where maxResults was used            and the results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=ListTaskDefinitionFamilies:
    get:
      summary: List Task Definition Families
      description: |-
        Returns a list of task definition families that are registered to your account
                    (which may include task definition families that no longer have any ACTIVE
                    task definition revisions).
      operationId: listTaskDefinitionFamilies
      x-api-path-slug: actionlisttaskdefinitionfamilies-get
      parameters:
      - in: query
        name: familyPrefix
        description: The familyPrefix is a string that is used to filter the results
          of                ListTaskDefinitionFamilies
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task definition family results returned
          by                ListTaskDefinitionFamilies in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTaskDefinitionFamilies
          request where maxResults was            used and the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: status
        description: The task definition family status with which to filter the                ListTaskDefinitionFamilies
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definition Families
  /?Action=ListTaskDefinitions:
    get:
      summary: List Task Definitions
      description: Returns a list of task definitions that are registered to your
        account.
      operationId: listTaskDefinitions
      x-api-path-slug: actionlisttaskdefinitions-get
      parameters:
      - in: query
        name: familyPrefix
        description: The full family name with which to filter the ListTaskDefinitions            results
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task definition results returned by                ListTaskDefinitions
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTaskDefinitions
          request where maxResults was used and            the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: sort
        description: The order in which to sort the results
        type: string
      - in: query
        name: status
        description: The task definition status with which to filter the                ListTaskDefinitions
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
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