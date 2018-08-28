{
  "info": {
    "name": "AWS CloudFormation API Describe Stacks",
    "_postman_id": "704842bb-dfb5-458a-867d-f9034aea30a0",
    "description": "Returns the description for the specified stack; if no stack name was specified, then it returns the description for all the stacks created.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stacks",
      "item": [
        {
          "id": "e0eca7d9-966a-4f69-a397-b4f1d7257fa3",
          "name": "cancelUpdateStack",
          "request": {
            "url": "http://example.com/api/?Action=CancelUpdateStack?StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an update on the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a4bec37-d658-47b0-a68e-69abbaef7223"
            }
          ]
        },
        {
          "id": "32b75df6-ed9c-408b-8bf5-de5ec458531b",
          "name": "createStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?Capabilities.member.N=Capabilities.member.N&DisableRollback=DisableRollback&NotificationARNs.member.N=NotificationARNs.member.N&OnFailure=OnFailure&Parameters.member.N=Parameters.member.N&ResourceTypes.member.N=ResourceTypes.member.N&RoleARN=RoleARN&StackName=StackName&StackPolicyBody=StackPolicyBody&StackPolicyURL=StackPolicyURL&Tags.member.N=Tags.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL&TimeoutInMinutes=TimeoutInMinutes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a stack as specified in the template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6793f501-0ad5-4386-8d39-2c752f588260"
            }
          ]
        },
        {
          "id": "0cfa60b1-2b14-4444-961d-ce7a567837b3",
          "name": "deleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?RetainResources.member.N=RetainResources.member.N&RoleARN=RoleARN&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73b5a42a-352a-4135-9cae-f96f8421fded"
            }
          ]
        },
        {
          "id": "4db10d33-7828-45d2-9205-fe4a23f4b02a",
          "name": "describeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the description for the specified stack; if no stack name was specified, then it returns the description for all the stacks created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99197ec7-5827-400a-9185-d58357adc1ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "8882cace-9973-4b3e-807d-d9ddb0ace4f3",
          "name": "continueUpdateRollback",
          "request": {
            "url": "http://example.com/api/?Action=ContinueUpdateRollback?ResourcesToSkip.member.N=ResourcesToSkip.member.N&RoleARN=RoleARN&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a specified stack that is in the UPDATE_ROLLBACK_FAILED state, continues rolling it back\n         to the UPDATE_ROLLBACK_COMPLETE state."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a82f49a0-b23d-4185-ad7f-e778368f28ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Sets",
      "item": [
        {
          "id": "21a448bb-26bd-4eec-9e43-6ff1e8c62efd",
          "name": "createChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateChangeSet?Capabilities.member.N=Capabilities.member.N&ChangeSetName=ChangeSetName&ChangeSetType=ChangeSetType&ClientToken=ClientToken&Description=Description&NotificationARNs.member.N=NotificationARNs.member.N&Parameters.member.N=Parameters.member.N&ResourceTypes.member.N=ResourceTypes.member.N&RoleARN=RoleARN&StackName=StackName&Tags.member.N=Tags.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL&UsePreviousTemplate=UsePreviousTemplate",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a list of changes for a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0234c8d-f1c0-4d4e-9705-fbbac9432388"
            }
          ]
        },
        {
          "id": "4159e0d5-f7b4-4cf9-aa90-4270d6364580",
          "name": "deleteChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteChangeSet?ChangeSetName=ChangeSetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified change set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fde8cb54-f3e2-476c-a711-fb689ef52889"
            }
          ]
        },
        {
          "id": "ae48e7d5-ed16-48c7-a6b4-f1561b1154ce",
          "name": "describeChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeChangeSet?ChangeSetName=ChangeSetName&NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the inputs for the change set and a list of changes that AWS CloudFormation will make if you execute the change set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb06620f-9f53-4554-b678-3894cc50da79"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Limits",
      "item": [
        {
          "id": "96954126-2486-4892-9b30-7e6268698199",
          "name": "describeAccountLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountLimits?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves your account's AWS CloudFormation limits, such as the maximum number of stacks that you can create in your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c49ef17f-746d-4556-bff1-5dfda2adec33"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Events",
      "item": [
        {
          "id": "b11f7061-5030-4edd-9a94-a3fe295fdc68",
          "name": "describeStackEvents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackEvents?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all stack related events for a specified stack in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ef9231a-3af1-4f39-9a0e-b42ee356aade"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Resources",
      "item": [
        {
          "id": "91767127-a425-4f99-8bdf-355bb42856cf",
          "name": "describeStackResource",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackResource?LogicalResourceId=LogicalResourceId&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the specified resource in the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0d20f32-754e-4d23-9931-26ffe83c71b5"
            }
          ]
        },
        {
          "id": "f3e9df81-c70b-4bdf-8075-c33ed5ff66a3",
          "name": "describeStackResources",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackResources?LogicalResourceId=LogicalResourceId&PhysicalResourceId=PhysicalResourceId&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns AWS resource descriptions for running and deleted stacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5aa054ab-49d4-4592-a44d-8851c01deb1f"
            }
          ]
        }
      ]
    }
  ]
}