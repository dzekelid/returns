---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Static Ip
  version: 1.0.0
  description: Returns information about a specific static IP.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetActiveNames:
    get:
      summary: Get Active Names
      description: Returns the names of all active (not deleted) resources.
      operationId: getActiveNames
      x-api-path-slug: actiongetactivenames-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for paginating results from your get active names
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Names
  /?Action=GetBlueprints:
    get:
      summary: Get Blueprints
      description: Returns the list of available instance images, or blueprints.
      operationId: getBlueprints
      x-api-path-slug: actiongetblueprints-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value indicating whether to include inactive results
          in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get blueprints      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetBundles:
    get:
      summary: Get Bundles
      description: Returns the list of bundles that are available for purchase.
      operationId: getBundles
      x-api-path-slug: actiongetbundles-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value that indicates whether to include inactive bundle
          results in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get bundles      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundles
  /?Action=GetDomain:
    get:
      summary: Get Domain
      description: Returns information about a specific domain recordset.
      operationId: getDomain
      x-api-path-slug: actiongetdomain-get
      parameters:
      - in: query
        name: domainName
        description: The domain name for which your want to return information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=GetDomains:
    get:
      summary: Get Domains
      description: Returns a list of all domains in the user's account.
      operationId: getDomains
      x-api-path-slug: actiongetdomains-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get domains      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=GetInstance:
    get:
      summary: Get Instance
      description: |-
        Returns information about a specific Amazon Lightsail instance, which is a virtual
              private server.
      operationId: getInstance
      x-api-path-slug: actiongetinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceAccessDetails:
    get:
      summary: Get Instance Access Details
      description: |-
        Returns temporary SSH keys you can use to connect to a specific virtual private server,
              or instance.
      operationId: getInstanceAccessDetails
      x-api-path-slug: actiongetinstanceaccessdetails-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to access
        type: string
      - in: query
        name: protocol
        description: The protocol to use to connect to your instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceMetricData:
    get:
      summary: Get Instance Metric Data
      description: |-
        Returns the data points for the specified Amazon Lightsail instance metric, given an
              instance name.
      operationId: getInstanceMetricData
      x-api-path-slug: actiongetinstancemetricdata-get
      parameters:
      - in: query
        name: endTime
        description: The end time of the time period
        type: string
      - in: query
        name: instanceName
        description: The name of the instance for which you want to get metrics data
        type: string
      - in: query
        name: metricName
        description: The metric name to get data about
        type: string
      - in: query
        name: period
        description: The time period for which you are requesting data
        type: string
      - in: query
        name: startTime
        description: The start time of the time period
        type: string
      - in: query
        name: statistics
        description: The instance statistics
        type: string
      - in: query
        name: unit
        description: The unit
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstancePortStates:
    get:
      summary: Get Instance Port States
      description: |-
        Returns the port states for a specific virtual private server, or
                instance.
      operationId: getInstancePortStates
      x-api-path-slug: actiongetinstanceportstates-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstances:
    get:
      summary: Get Instances
      description: |-
        Returns information about all Amazon Lightsail virtual private servers, or
                instances.
      operationId: getInstances
      x-api-path-slug: actiongetinstances-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get instances      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceSnapshot:
    get:
      summary: Get Instance Snapshot
      description: Returns information about a specific instance snapshot.
      operationId: getInstanceSnapshot
      x-api-path-slug: actiongetinstancesnapshot-get
      parameters:
      - in: query
        name: instanceSnapshotName
        description: The name of the snapshot for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceSnapshots:
    get:
      summary: Get Instance Snapshots
      description: Returns all instance snapshots for the user's account.
      operationId: getInstanceSnapshots
      x-api-path-slug: actiongetinstancesnapshots-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get instance snapshots      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceState:
    get:
      summary: Get Instance State
      description: Returns the state of a specific instance.
      operationId: getInstanceState
      x-api-path-slug: actiongetinstancestate-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to get state information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetKeyPair:
    get:
      summary: Get Key Pair
      description: Returns information about a specific key pair.
      operationId: getKeyPair
      x-api-path-slug: actiongetkeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name of the key pair for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=GetKeyPairs:
    get:
      summary: Get Key Pairs
      description: Returns information about all key pairs in the user's account.
      operationId: getKeyPairs
      x-api-path-slug: actiongetkeypairs-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get key pairs      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=GetOperation:
    get:
      summary: Get Operation
      description: Returns information about a specific operation.
      operationId: getOperation
      x-api-path-slug: actiongetoperation-get
      parameters:
      - in: query
        name: operationId
        description: A GUID used to identify the operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Operations
  /?Action=GetOperations:
    get:
      summary: Get Operations
      description: Returns information about all operations.
      operationId: getOperations
      x-api-path-slug: actiongetoperations-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get operations      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Operations
  /?Action=GetRegions:
    get:
      summary: Get Regions
      description: Returns a list of all valid regions for Amazon Lightsail.
      operationId: getRegions
      x-api-path-slug: actiongetregions-get
      parameters:
      - in: query
        name: includeAvailabilityZones
        description: A Boolean value indicating whether to also include Availability
          Zones in your get      regions request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Regions
  /?Action=GetStaticIp:
    get:
      summary: Get Static Ip
      description: Returns information about a specific static IP.
      operationId: getStaticIp
      x-api-path-slug: actiongetstaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP in Lightsail
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
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