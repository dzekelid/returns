---
swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 0
info:
  title: AWS Simple Notification Service API List Phone Numbers Opted Out
  version: 1.0.0
  description: Returns a list of phone numbers that are opted out, meaning you cannot
    send SMS messages to them.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetSMSAttributes:
    get:
      summary: Get S M S Attributes
      description: Returns the settings for sending SMS messages from your account.
      operationId: getSMSAttributes
      x-api-path-slug: actiongetsmsattributes-get
      parameters:
      - in: query
        name: attributes.member.N
        description: A list of the individual attribute names, such as MonthlySpendLimit,
          for which      you want values
        type: string
      responses:
        200:
          description: OK
      tags:
      - SMS
  /?Action=GetSubscriptionAttributes:
    get:
      summary: Get Subscription Attributes
      description: Returns all of the properties of a subscription.
      operationId: getSubscriptionAttributes
      x-api-path-slug: actiongetsubscriptionattributes-get
      parameters:
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=GetTopicAttributes:
    get:
      summary: Get Topic Attributes
      description: Returns all of the properties of a topic.
      operationId: getTopicAttributes
      x-api-path-slug: actiongettopicattributes-get
      parameters:
      - in: query
        name: TopicArn
        description: The ARN of the topic whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=ListPhoneNumbersOptedOut:
    get:
      summary: List Phone Numbers Opted Out
      description: Returns a list of phone numbers that are opted out, meaning you
        cannot send SMS messages to them.
      operationId: listPhoneNumbersOptedOut
      x-api-path-slug: actionlistphonenumbersoptedout-get
      parameters:
      - in: query
        name: nextToken
        description: A NextToken string is used when you call the      ListPhoneNumbersOptedOut
          action to retrieve additional records that are      available after the
          first page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Opt Out
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