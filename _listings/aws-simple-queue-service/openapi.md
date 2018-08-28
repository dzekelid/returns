swagger: "2.0"
x-collection-name: AWS Simple Queue Service
x-complete: 1
info:
  title: AWS Simple Queue Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetQueueUrl:
    get:
      summary: Get Queue Url
      description: Returns the URL of an existing queue.
      operationId: getQueueUrl
      x-api-path-slug: actiongetqueueurl-get
      parameters:
      - in: query
        name: QueueName
        description: The name of the queue whose URL must be fetched
        type: string
      - in: query
        name: QueueOwnerAWSAccountId
        description: The AWS account ID of the account that created the queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=ListDeadLetterSourceQueues:
    get:
      summary: List Dead Letter Source Queues
      description: Returns a list of your queues that have the RedrivePolicy queue
        attribute configured with a dead letter queue.
      operationId: listDeadLetterSourceQueues
      x-api-path-slug: actionlistdeadlettersourcequeues-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of a dead letter queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=ListQueues:
    get:
      summary: List Queues
      description: Returns a list of your queues.
      operationId: listQueues
      x-api-path-slug: actionlistqueues-get
      parameters:
      - in: query
        name: QueueNamePrefix
        description: A string to use for filtering the list results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues