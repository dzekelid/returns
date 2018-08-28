---
swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 0
info:
  title: AWS WAF API List Byte Match Sets
  version: 1.0.0
  description: 'Service: AWS WAFReturns an array of.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetByteMatchSet:
    get:
      summary: Get Byte Match Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getByteMatchSet
      x-api-path-slug: actiongetbytematchset-get
      parameters:
      - in: query
        name: ByteMatchSetId
        description: The ByteMatchSetId of the ByteMatchSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Set
  /?Action=GetChangeTokenStatus:
    get:
      summary: Get Change Token Status
      description: 'Service: AWS WAFReturns the status of a ChangeToken that you got
        by calling.'
      operationId: getChangeTokenStatus
      x-api-path-slug: actiongetchangetokenstatus-get
      parameters:
      - in: query
        name: ChangeToken
        description: The change token for which you want to get the status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Token
  /?Action=GetIPSet:
    get:
      summary: Get IP Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getIPSet
      x-api-path-slug: actiongetipset-get
      parameters:
      - in: query
        name: IPSetId
        description: The IPSetId of the IPSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Sets
  /?Action=GetRule:
    get:
      summary: Get Rule
      description: 'Service: AWS WAFReturns the.'
      operationId: getRule
      x-api-path-slug: actiongetrule-get
      parameters:
      - in: query
        name: RuleId
        description: The RuleId of the Rule that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=GetSizeConstraintSet:
    get:
      summary: Get Size Constraint Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getSizeConstraintSet
      x-api-path-slug: actiongetsizeconstraintset-get
      parameters:
      - in: query
        name: SizeConstraintSetId
        description: The SizeConstraintSetId of the SizeConstraintSet that you want
          to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Size Constraint Set
  /?Action=GetSqlInjectionMatchSet:
    get:
      summary: Get Sql Injection Match Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getSqlInjectionMatchSet
      x-api-path-slug: actiongetsqlinjectionmatchset-get
      parameters:
      - in: query
        name: SqlInjectionMatchSetId
        description: The SqlInjectionMatchSetId of the SqlInjectionMatchSet that you
          want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - SQL Injection Match Set
  /?Action=GetWebACL:
    get:
      summary: Get Web ACL
      description: 'Service: AWS WAFReturns the.'
      operationId: getWebACL
      x-api-path-slug: actiongetwebacl-get
      parameters:
      - in: query
        name: WebACLId
        description: The WebACLId of the WebACL that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=GetWebACLForResource:
    get:
      summary: Get Web ACLFor Resource
      description: 'Service: AWS WAF RegionalReturns the web ACL for the specified
        resource.'
      operationId: getWebACLForResource
      x-api-path-slug: actiongetwebaclforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource for which to get
          the web ACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=GetXssMatchSet:
    get:
      summary: Get Xss Match Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getXssMatchSet
      x-api-path-slug: actiongetxssmatchset-get
      parameters:
      - in: query
        name: XssMatchSetId
        description: The XssMatchSetId of the XssMatchSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - XSS Match Set
  /?Action=ListByteMatchSets:
    get:
      summary: List Byte Match Sets
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listByteMatchSets
      x-api-path-slug: actionlistbytematchsets-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of ByteMatchSet objects that you want AWS
          WAF to return for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more ByteMatchSets
          than the value of Limit, AWS WAF returns a NextMarker value in the response
          that allows you to list another group of ByteMatchSets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Sets
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