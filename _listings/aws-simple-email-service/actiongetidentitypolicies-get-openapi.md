---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Get Identity Policies
  version: 1.0.0
  description: Returns the requested sending authorization policies for the given
    identity (an email address or a domain).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeActiveReceiptRuleSet:
    get:
      summary: Describe Active Receipt Rule Set
      description: Returns the metadata and receipt rules for the receipt rule set
        that is currently active.
      operationId: describeActiveReceiptRuleSet
      x-api-path-slug: actiondescribeactivereceiptruleset-get
      parameters:
      - in: query
        name: Metadata
        description: The metadata for the currently active receipt rule set
        type: string
      - in: query
        name: Rules.member.N
        description: The receipt rules that belong to the active rule set
        type: string
      responses:
        200:
          description: OK
      tags:
      - Receipt Rule Sets
  /?Action=DescribeConfigurationSet:
    get:
      summary: Describe Configuration Set
      description: Returns the details of the specified configuration set.
      operationId: describeConfigurationSet
      x-api-path-slug: actiondescribeconfigurationset-get
      parameters:
      - in: query
        name: ConfigurationSetAttributeNames.member.N
        description: A list of configuration set attributes to return
        type: string
      - in: query
        name: ConfigurationSetName
        description: The name of the configuration set to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Sets
  /?Action=DescribeReceiptRule:
    get:
      summary: Describe Receipt Rule
      description: Returns the details of the specified receipt rule.
      operationId: describeReceiptRule
      x-api-path-slug: actiondescribereceiptrule-get
      parameters:
      - in: query
        name: RuleName
        description: The name of the receipt rule
        type: string
      - in: query
        name: RuleSetName
        description: The name of the receipt rule set to which the receipt rule belongs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Receipt Rules
  /?Action=DescribeReceiptRuleSet:
    get:
      summary: Describe Receipt Rule Set
      description: Returns the details of the specified receipt rule set.
      operationId: describeReceiptRuleSet
      x-api-path-slug: actiondescribereceiptruleset-get
      parameters:
      - in: query
        name: RuleSetName
        description: The name of the receipt rule set to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Receipt Rule Sets
  /?Action=GetIdentityDkimAttributes:
    get:
      summary: Get Identity Dkim Attributes
      description: Returns the current status of Easy DKIM signing for an entity.
      operationId: getIdentityDkimAttributes
      x-api-path-slug: actiongetidentitydkimattributes-get
      parameters:
      - in: query
        name: Identities.member.N
        description: A list of one or more verified identities - email addresses,
          domains, or both
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=GetIdentityMailFromDomainAttributes:
    get:
      summary: Get Identity Mail From Domain Attributes
      description: Returns the custom MAIL FROM attributes for a list of identities
        (email addresses and/or domains).
      operationId: getIdentityMailFromDomainAttributes
      x-api-path-slug: actiongetidentitymailfromdomainattributes-get
      parameters:
      - in: query
        name: Identities.member.N
        description: A list of one or more identities
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=GetIdentityPolicies:
    get:
      summary: Get Identity Policies
      description: Returns the requested sending authorization policies for the given
        identity (an email address or a domain).
      operationId: getIdentityPolicies
      x-api-path-slug: actiongetidentitypolicies-get
      parameters:
      - in: query
        name: Identity
        description: The identity for which the policies will be retrieved
        type: string
      - in: query
        name: PolicyNames.member.N
        description: A list of the names of policies to be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
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