---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Describe Tags
  version: 1.0.0
  description: Returns a list of tags.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeClusterParameterGroups:
    get:
      summary: Describe Cluster Parameter Groups
      description: |-
        Returns a list of Amazon Redshift parameter groups, including parameter groups you
                    created and the default parameter group.
      operationId: describeClusterParameterGroups
      x-api-path-slug: actiondescribeclusterparametergroups-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a specific parameter group for which to return details
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          parameter            groups that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster parameter            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DescribeClusterParameters:
    get:
      summary: Describe Cluster Parameters
      description: |-
        Returns a detailed list of parameters contained within the specified Amazon Redshift
                    parameter group.
      operationId: describeClusterParameters
      x-api-path-slug: actiondescribeclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a cluster parameter group for which to return details
        type: string
      - in: query
        name: Source
        description: The parameter types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeClusters:
    get:
      summary: Describe Clusters
      description: |-
        Returns properties of provisioned clusters including general cluster properties,
                    cluster database properties, maintenance and backup properties, and security and access
                    properties.
      operationId: describeClusters
      x-api-path-slug: actiondescribeclusters-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of a cluster whose properties you are requesting
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching clusters
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          clusters that are            associated with the specified tag value or
          values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeClusterSecurityGroups:
    get:
      summary: Describe Cluster Security Groups
      description: Returns information about Amazon Redshift security groups.
      operationId: describeClusterSecurityGroups
      x-api-path-slug: actiondescribeclustersecuritygroups-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of a cluster security group for which you are requesting
          details
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          security groups            that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster security            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DescribeClusterSnapshots:
    get:
      summary: Describe Cluster Snapshots
      description: |-
        Returns one or more snapshot objects, which contain metadata about your cluster
                    snapshots.
      operationId: describeClusterSnapshots
      x-api-path-slug: actiondescribeclustersnapshots-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster for which information about snapshots
          is            requested
        type: string
      - in: query
        name: EndTime
        description: A time value that requests only snapshots created at or before
          the specified time
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: OwnerAccount
        description: The AWS customer account used to create or copy the snapshot
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The snapshot identifier of the snapshot about which to return            information
        type: string
      - in: query
        name: SnapshotType
        description: The type of snapshots for which you are requesting information
        type: string
      - in: query
        name: StartTime
        description: A value that requests only snapshots created at or after the
          specified time
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          snapshots that            are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster snapshots            that are associated with the specified tag
          value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeClusterSubnetGroups:
    get:
      summary: Describe Cluster Subnet Groups
      description: |-
        Returns one or more cluster subnet group objects, which contain metadata about your
                    cluster subnet groups.
      operationId: describeClusterSubnetGroups
      x-api-path-slug: actiondescribeclustersubnetgroups-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group for which information is
          requested
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          subnet groups            that are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster subnet            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DescribeClusterVersions:
    get:
      summary: Describe Cluster Versions
      description: Returns descriptions of the available Amazon Redshift cluster versions.
      operationId: describeClusterVersions
      x-api-path-slug: actiondescribeclusterversions-get
      parameters:
      - in: query
        name: ClusterParameterGroupFamily
        description: The name of a specific cluster parameter group family to return
          details            for
        type: string
      - in: query
        name: ClusterVersion
        description: The specific cluster version to return
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeDefaultClusterParameters:
    get:
      summary: Describe Default Cluster Parameters
      description: |-
        Returns a list of parameter settings for the specified parameter group
                    family.
      operationId: describeDefaultClusterParameters
      x-api-path-slug: actiondescribedefaultclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The name of the cluster parameter group family
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeEvents:
    get:
      summary: Describe Events
      description: |-
        Returns events related to clusters, security groups, snapshots, and parameter
                    groups for the past 14 days.
      operationId: describeEvents
      x-api-path-slug: actiondescribeevents-get
      parameters:
      - in: query
        name: Duration
        description: The number of minutes prior to the time of the request for which
          to retrieve            events
        type: string
      - in: query
        name: EndTime
        description: The end of the time interval for which to retrieve events, specified
          in ISO 8601            format
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source for which events will be returned
        type: string
      - in: query
        name: SourceType
        description: The event source to retrieve events for
        type: string
      - in: query
        name: StartTime
        description: The beginning of the time interval to retrieve events for, specified
          in ISO 8601            format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=DescribeHsmClientCertificates:
    get:
      summary: Describe Hsm Client Certificates
      description: Returns information about the specified HSM client certificate.
      operationId: describeHsmClientCertificates
      x-api-path-slug: actiondescribehsmclientcertificates-get
      parameters:
      - in: query
        name: HsmClientCertificateIdentifier
        description: The identifier of a specific HSM client certificate for which
          you want information
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching HSM
          client certificates            that are associated with the specified key
          or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          HSM client            certificates that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Client Certificates
  /?Action=DescribeHsmConfigurations:
    get:
      summary: Describe Hsm Configurations
      description: Returns information about the specified Amazon Redshift HSM configuration.
      operationId: describeHsmConfigurations
      x-api-path-slug: actiondescribehsmconfigurations-get
      parameters:
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier of a specific Amazon Redshift HSM configuration
          to be described
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching HSM
          configurations that            are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          HSM configurations            that are associated with the specified tag
          value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
  /?Action=DescribeOrderableClusterOptions:
    get:
      summary: Describe Orderable Cluster Options
      description: Returns a list of orderable cluster options.
      operationId: describeOrderableClusterOptions
      x-api-path-slug: actiondescribeorderableclusteroptions-get
      parameters:
      - in: query
        name: ClusterVersion
        description: The version filter value
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: NodeType
        description: The node type filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Options
  /?Action=DescribeReservedNodeOfferings:
    get:
      summary: Describe Reserved Node Offerings
      description: |-
        Returns a list of the available reserved node offerings by Amazon Redshift with their
                    descriptions including the node type, the fixed and recurring costs of reserving the
                    node and duration the node will be reserved for you.
      operationId: describeReservedNodeOfferings
      x-api-path-slug: actiondescribereservednodeofferings-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ReservedNodeOfferingId
        description: The unique identifier for the offering
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Nodes
  /?Action=DescribeReservedNodes:
    get:
      summary: Describe Reserved Nodes
      description: Returns the descriptions of the reserved nodes.
      operationId: describeReservedNodes
      x-api-path-slug: actiondescribereservednodes-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ReservedNodeId
        description: Identifier for the node reservation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Nodes
  /?Action=DescribeResize:
    get:
      summary: Describe Resize
      description: Returns information about the last resize operation for the specified
        cluster.
      operationId: describeResize
      x-api-path-slug: actiondescriberesize-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of a cluster whose resize progress you
          are requesting
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resize
  /?Action=DescribeSnapshotCopyGrants:
    get:
      summary: Describe Snapshot Copy Grants
      description: |-
        Returns a list of snapshot copy grants owned by the AWS account in the destination
                    region.
      operationId: describeSnapshotCopyGrants
      x-api-path-slug: actiondescribesnapshotcopygrants-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching resources
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          resources that are            associated with the specified value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Returns a list of tags.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: Marker
        description: A value that indicates the starting point for the next set of
          response records in a            subsequent request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number or response records to return in each call
        type: string
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) for which you want to describe
          the tag or tags
        type: string
      - in: query
        name: ResourceType
        description: The type of resource with which you want to view tags
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching resources
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          resources that are            associated with the specified value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
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