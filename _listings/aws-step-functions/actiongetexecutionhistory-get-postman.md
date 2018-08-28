{
  "info": {
    "name": "AWS Step Functions API Get Execution History",
    "_postman_id": "0bdb38cf-d6b8-4b94-80a8-6a811eadf5ee",
    "description": "Returns the history of the specified execution as a list of events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "afbde3ee-9248-41ec-bb15-68d25594ad2e",
          "name": "createActivity",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivity?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "704b1283-c7ac-4f20-8d55-c65c8b1bd404"
            }
          ]
        },
        {
          "id": "f94165e2-7c37-4f50-9f0f-c966bcdfe5d9",
          "name": "deleteActivity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivity?activityArn=activityArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca51d5a4-02cb-4e2a-8773-c59b741b798a"
            }
          ]
        },
        {
          "id": "5044f876-1429-482c-a049-ecabcf7ba60a",
          "name": "describeActivity",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivity?activityArn=activityArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f96b83bc-bec8-4012-84d6-537ec5eb69d5"
            }
          ]
        }
      ]
    },
    {
      "name": "State Machine",
      "item": [
        {
          "id": "e61fc89a-bbc4-4823-815e-5cb63027f2fc",
          "name": "createStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=CreateStateMachine?definition=definition&name=name&roleArn=roleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8312429-40bc-419a-bbf1-48e695f9c35f"
            }
          ]
        },
        {
          "id": "b50e1b49-a7aa-4494-b3ae-dd1ca9d78dba",
          "name": "deleteStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStateMachine?stateMachineArn=stateMachineArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f43266a8-ab8a-4660-899e-613e317b2875"
            }
          ]
        },
        {
          "id": "486676ed-00fb-480d-b02d-142fde3123b1",
          "name": "describeStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStateMachine?stateMachineArn=stateMachineArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aed300cd-f27d-4a1e-a891-a218dcf00faf"
            }
          ]
        }
      ]
    },
    {
      "name": "Execution",
      "item": [
        {
          "id": "820d88a7-b3bc-4626-a5e3-d99b2fe942a1",
          "name": "describeExecution",
          "request": {
            "url": "http://example.com/api/?Action=DescribeExecution?executionArn=executionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes an execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cce481df-ea46-4671-a110-d69a2a297db3"
            }
          ]
        },
        {
          "id": "8da92382-b146-4e7d-907f-fe8e6c2d4a7d",
          "name": "getExecutionHistory",
          "request": {
            "url": "http://example.com/api/?Action=GetExecutionHistory?executionArn=executionArn&maxResults=maxResults&nextToken=nextToken&reverseOrder=reverseOrder",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the history of the specified execution as a list of events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c2e261f-6bbc-4048-89d2-e158b69453bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity Task",
      "item": [
        {
          "id": "762b0eb0-a599-4abb-b944-11cccdfb6398",
          "name": "getActivityTask",
          "request": {
            "url": "http://example.com/api/?Action=GetActivityTask?activityArn=activityArn&workerName=workerName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Used by workers to retrieve a task (with the specified activity ARN) which has been scheduled \n    for execution by a running state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcace727-53ac-41c5-8981-4cbf68b49b8d"
            }
          ]
        }
      ]
    }
  ]
}