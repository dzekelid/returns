swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 1
info:
  title: AWS Simple Notification Service API
  version: 1.0.0
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
  /?Action=ListSubscriptions:
    get:
      summary: List Subscriptions
      description: Returns a list of the requester's subscriptions.
      operationId: listSubscriptions
      x-api-path-slug: actionlistsubscriptions-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptions request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListSubscriptionsByTopic:
    get:
      summary: List Subscriptions By Topic
      description: Returns a list of the subscriptions to a specific topic.
      operationId: listSubscriptionsByTopic
      x-api-path-slug: actionlistsubscriptionsbytopic-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptionsByTopic request
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to find subscriptions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListTopics:
    get:
      summary: List Topics
      description: Returns a list of the requester's topics.
      operationId: listTopics
      x-api-path-slug: actionlisttopics-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListTopics request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics