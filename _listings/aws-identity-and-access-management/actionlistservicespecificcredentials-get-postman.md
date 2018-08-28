{
  "info": {
    "name": "AWS Identity and Access Management API List Service Specific Credentials",
    "_postman_id": "67e9cd5f-6cab-4379-9b29-5938da6da94c",
    "description": "Returns information about the service-specific credentials associated with the\n      specified IAM user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "OpenID Connect Providers",
      "item": [
        {
          "id": "ec829804-e623-4661-9bf6-bb9b86d753b8",
          "name": "addClientIDToOpenIDConnectProvider",
          "request": {
            "url": "http://example.com/api/?Action=AddClientIDToOpenIDConnectProvider?ClientID=ClientID&OpenIDConnectProviderArn=OpenIDConnectProviderArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new client ID (also known as audience) to the list of client IDs already\n      registered for the specified IAM OpenID Connect (OIDC) provider resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0296080-4ddd-4ca1-ac58-1409c2ce939b"
            }
          ]
        },
        {
          "id": "6131ba55-f109-48f0-9f34-69d17218da93",
          "name": "createOpenIDConnectProvider",
          "request": {
            "url": "http://example.com/api/?Action=CreateOpenIDConnectProvider?ClientIDList.member.N=ClientIDList.member.N&ThumbprintList.member.N=ThumbprintList.member.N&Url=Url",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an IAM entity to describe an identity provider (IdP) that supports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d43883e4-d2b5-4547-b171-b3fa44c42bb5"
            }
          ]
        },
        {
          "id": "e052eb92-a5db-490b-b492-e613be83903b",
          "name": "deleteOpenIDConnectProvider",
          "request": {
            "url": "http://example.com/api/?Action=DeleteOpenIDConnectProvider?OpenIDConnectProviderArn=OpenIDConnectProviderArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an OpenID Connect identity provider (IdP) resource object in IAM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49e8af86-4af1-417a-81df-e7e900c65137"
            }
          ]
        },
        {
          "id": "02a8e603-9f14-4838-9cb8-a28c73691cb7",
          "name": "getOpenIDConnectProvider",
          "request": {
            "url": "http://example.com/api/?Action=GetOpenIDConnectProvider?OpenIDConnectProviderArn=OpenIDConnectProviderArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the specified OpenID Connect (OIDC) provider resource object\n      in IAM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4409573a-45d8-4a1f-9df0-0ce21eae5f7a"
            }
          ]
        },
        {
          "id": "d91196f3-3b0c-4aa0-a67c-56b6e4bc6c3f",
          "name": "listOpenIDConnectProviders",
          "request": {
            "url": "http://example.com/api/?Action=ListOpenIDConnectProviders?OpenIDConnectProviderList.member.N=OpenIDConnectProviderList.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists information about the IAM OpenID Connect (OIDC) provider resource objects\n      defined in the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4233c48d-e47a-457f-9b36-c3b0c0d4580a"
            }
          ]
        }
      ]
    },
    {
      "name": "Role Instance",
      "item": [
        {
          "id": "f63f323d-e043-4c81-9530-0b9dfef11d62",
          "name": "addRoleToInstanceProfile",
          "request": {
            "url": "http://example.com/api/?Action=AddRoleToInstanceProfile?InstanceProfileName=InstanceProfileName&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified IAM role to the specified instance profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "daa0c309-df8c-46e0-9d48-04ff18a690d3"
            }
          ]
        }
      ]
    },
    {
      "name": "User Groups",
      "item": [
        {
          "id": "57cec363-f967-4077-8f09-44b66a05916a",
          "name": "addUserToGroup",
          "request": {
            "url": "http://example.com/api/?Action=AddUserToGroup?GroupName=GroupName&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified user to the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a5f7dc0-4c99-4d5a-81dd-57c4ce138c64"
            }
          ]
        }
      ]
    },
    {
      "name": "Group Policies",
      "item": [
        {
          "id": "28bbc53e-6cc6-4ddd-b40d-aa4042dc053f",
          "name": "attachGroupPolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachGroupPolicy?GroupName=GroupName&PolicyArn=PolicyArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified managed policy to the specified IAM group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1c0129f-65cd-4d40-ab21-d3783e6dc0da"
            }
          ]
        },
        {
          "id": "7cae8273-dd4e-4d6a-8523-07bb4fbccefd",
          "name": "deleteGroupPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGroupPolicy?GroupName=GroupName&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified inline policy that is embedded in the specified IAM\n      group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16ef97e5-a0dc-490f-8fd9-89a84a628b98"
            }
          ]
        },
        {
          "id": "cf93d8ef-656c-42b9-b630-0751ff5885d8",
          "name": "detachGroupPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DetachGroupPolicy?GroupName=GroupName&PolicyArn=PolicyArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified managed policy from the specified IAM group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46de5e45-7831-4c64-b3ee-427070cc80af"
            }
          ]
        },
        {
          "id": "9c2e6f61-6b81-486c-b850-80c9311c2eb7",
          "name": "getGroupPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetGroupPolicy?GroupName=GroupName&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified inline policy document that is embedded in the specified IAM\n      group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e89da4c-231d-4d63-b8da-67c012bd9cb5"
            }
          ]
        },
        {
          "id": "e85e135b-3fae-4821-8d10-9b9fc225b44e",
          "name": "listGroupPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListGroupPolicies?GroupName=GroupName&Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the names of the inline policies that are embedded in the specified IAM\n      group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "776b1496-3fa8-4d1d-aea1-0b4cff122795"
            }
          ]
        }
      ]
    },
    {
      "name": "Role Policies",
      "item": [
        {
          "id": "069606c1-91b6-4a12-8d66-ae89d042a9cc",
          "name": "attachRolePolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachRolePolicy?PolicyArn=PolicyArn&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified managed policy to the specified IAM role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a8d5017-a931-4b69-8b4c-7bcc8a84dc89"
            }
          ]
        },
        {
          "id": "6b16641e-5a87-4151-a44f-627bb918bc09",
          "name": "deleteRolePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRolePolicy?PolicyName=PolicyName&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified inline policy that is embedded in the specified IAM\n      role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad39adec-f798-42dd-bc0c-93d6c5685246"
            }
          ]
        },
        {
          "id": "a528cf55-3ad3-4150-accc-cfd386235a71",
          "name": "detachRolePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DetachRolePolicy?PolicyArn=PolicyArn&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified managed policy from the specified role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e617270-8bc1-4062-8bd4-11daae0cb026"
            }
          ]
        },
        {
          "id": "c6fdcac6-6698-491b-8eb8-9fe8903db088",
          "name": "getRolePolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetRolePolicy?PolicyName=PolicyName&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified inline policy document that is embedded with the specified\n      IAM role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bbdad0e-76a6-45ea-be8b-b4396c3220cb"
            }
          ]
        },
        {
          "id": "b8897881-dc63-414f-9894-2f15dd6590fa",
          "name": "listRolePolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListRolePolicies?Marker=Marker&MaxItems=MaxItems&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the names of the inline policies that are embedded in the specified IAM\n      role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cda9e36b-d25a-431b-a96c-90d752898719"
            }
          ]
        }
      ]
    },
    {
      "name": "User Policies",
      "item": [
        {
          "id": "46521388-696d-4cbc-94e7-0c28dc8e69bf",
          "name": "attachUserPolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachUserPolicy?PolicyArn=PolicyArn&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified managed policy to the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "674ee588-a855-4238-8d48-6e49ac50f318"
            }
          ]
        },
        {
          "id": "b0a2977b-f7b7-4ed1-8c5e-e130cd9ee2f5",
          "name": "deleteUserPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPolicy?PolicyName=PolicyName&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified inline policy that is embedded in the specified IAM\n      user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b96f789-fc19-4b25-9ee1-e42b9b450912"
            }
          ]
        },
        {
          "id": "05761306-ddd1-4f98-9e81-a9dddb6210c3",
          "name": "detachUserPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DetachUserPolicy?PolicyArn=PolicyArn&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified managed policy from the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cdd1c66-54b3-400e-9e9a-af4f060047c1"
            }
          ]
        },
        {
          "id": "baccb165-3759-4b87-b84a-4a8a0f0c6f8c",
          "name": "getUserPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetUserPolicy?PolicyName=PolicyName&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified inline policy document that is embedded in the specified IAM\n      user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f52ab043-81b6-496d-b7fd-13bc8442602e"
            }
          ]
        }
      ]
    },
    {
      "name": "Passwords",
      "item": [
        {
          "id": "777698d4-406e-440c-8572-8eee8216da8c",
          "name": "changePassword",
          "request": {
            "url": "http://example.com/api/?Action=ChangePassword?NewPassword=NewPassword&OldPassword=OldPassword",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the password of the IAM user who is calling this action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a497e8db-674b-4216-a399-acdc795d6fda"
            }
          ]
        }
      ]
    },
    {
      "name": "Access Keys",
      "item": [
        {
          "id": "972e5089-94a4-445c-be12-323298877d54",
          "name": "createAccessKey",
          "request": {
            "url": "http://example.com/api/?Action=CreateAccessKey?UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new AWS secret access key and corresponding AWS access key ID for the\n      specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cf5d806-7715-40fc-ab9e-b755dba2c383"
            }
          ]
        },
        {
          "id": "13d04c14-22d9-4307-bf73-d280de9e6873",
          "name": "deleteAccessKey",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAccessKey?AccessKeyId=AccessKeyId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the access key pair associated with the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "376b7c2a-9a0d-459a-a6d1-c716057d4cc5"
            }
          ]
        },
        {
          "id": "8f841d64-fe16-403e-a804-fcd0501143b0",
          "name": "getAccessKeyLastUsed",
          "request": {
            "url": "http://example.com/api/?Action=GetAccessKeyLastUsed?AccessKeyId=AccessKeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about when the specified access key was last used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd7dd0f7-0745-4c65-a148-5798c39a2aa0"
            }
          ]
        },
        {
          "id": "15307194-3c03-41b6-b85e-573d0ed4270c",
          "name": "listAccessKeys",
          "request": {
            "url": "http://example.com/api/?Action=ListAccessKeys?Marker=Marker&MaxItems=MaxItems&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the access key IDs associated with the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd6f3c72-a738-4538-adde-295be91b03ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Alias",
      "item": [
        {
          "id": "6fc9e28c-2f7d-4d95-bc5c-a5699c1323aa",
          "name": "createAccountAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAccountAlias?AccountAlias=AccountAlias",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d8b7e31-bec1-47cb-a60e-bd87dd56160e"
            }
          ]
        },
        {
          "id": "cdb8be11-9a7f-439e-8dec-a797b021f779",
          "name": "deleteAccountAlias",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAccountAlias?AccountAlias=AccountAlias",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified AWS account alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92c816cd-fa0a-43b0-9adf-461a56e2340f"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "53391c3f-3baa-4c8c-b5c3-b493665022e0",
          "name": "createGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateGroup?GroupName=GroupName&Path=Path",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b520ab5f-b419-441b-8c0b-e647a4cc8816"
            }
          ]
        },
        {
          "id": "442a894c-60f6-4a6f-b7bb-e23abfbadd5f",
          "name": "deleteGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGroup?GroupName=GroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IAM group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90029fd1-1d82-4dc6-a1c8-2104e795478b"
            }
          ]
        },
        {
          "id": "711818c8-3e98-4239-9bf7-d12ce17d71d2",
          "name": "getGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetGroup?GroupName=GroupName&Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of IAM users that are in the specified IAM group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5393f5f-f288-463d-9562-4b5435dcda91"
            }
          ]
        },
        {
          "id": "e1e9f636-c1ef-4ee0-a4f5-dca60a1896cf",
          "name": "listGroups",
          "request": {
            "url": "http://example.com/api/?Action=ListGroups?Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IAM groups that have the specified path prefix."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e2ce8e1-d9b1-4494-ac4d-b9042669c3f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance Profiles",
      "item": [
        {
          "id": "af7d61b7-c56c-40f7-9e7d-9016aa700cbf",
          "name": "createInstanceProfile",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstanceProfile?InstanceProfileName=InstanceProfileName&Path=Path",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new instance profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce15af14-1e68-4a43-b792-04929bc1c4ec"
            }
          ]
        },
        {
          "id": "0eb4168d-f448-4c82-ac4a-73e661a8886d",
          "name": "deleteInstanceProfile",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInstanceProfile?InstanceProfileName=InstanceProfileName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified instance profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7aaf2852-487d-4313-a93b-0ebecc1b3b50"
            }
          ]
        },
        {
          "id": "2489a18c-fc41-432e-90c7-fdb34b5fe8aa",
          "name": "getInstanceProfile",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceProfile?InstanceProfileName=InstanceProfileName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the specified instance profile, including the instance\n      profile's path, GUID, ARN, and role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1766d589-1d0f-4d3b-90ad-7ea9b6e78200"
            }
          ]
        },
        {
          "id": "96a25cee-81cd-44ba-bf70-a07a3429a701",
          "name": "listInstanceProfiles",
          "request": {
            "url": "http://example.com/api/?Action=ListInstanceProfiles?Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the instance profiles that have the specified path prefix."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26401b16-1e9c-46b6-b579-fb2f0e0efd0f"
            }
          ]
        }
      ]
    },
    {
      "name": "Login Profiles",
      "item": [
        {
          "id": "6473739f-7277-4833-8baa-9ae20353f8e0",
          "name": "createLoginProfile",
          "request": {
            "url": "http://example.com/api/?Action=CreateLoginProfile?Password=Password&PasswordResetRequired=PasswordResetRequired&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a password for the specified user, giving the user the ability to access AWS\n      services through the AWS Management Console."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc062527-601c-458c-ace5-126b4de305ec"
            }
          ]
        },
        {
          "id": "0d56754e-a6f9-4e20-988d-c355346ad7f7",
          "name": "deleteLoginProfile",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLoginProfile?UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the password for the specified IAM user, which terminates the user's ability\n      to access AWS services through the AWS Management Console."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e923d4c-05fd-47b7-b913-2f19819975d6"
            }
          ]
        },
        {
          "id": "9e713f7e-0b66-4266-a62f-fd92a17eea49",
          "name": "getLoginProfile",
          "request": {
            "url": "http://example.com/api/?Action=GetLoginProfile?UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the user name and password-creation date for the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8fd2e9d3-a081-410e-a73a-c854c8cc7134"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "51f20553-a917-4fd5-be25-4243fbe91a00",
          "name": "createPolicy",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicy?Description=Description&Path=Path&PolicyDocument=PolicyDocument&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new managed policy for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e8e0030-9c6e-4fa0-b5b3-9d2fc2492703"
            }
          ]
        },
        {
          "id": "00fa5fe4-7c68-4ec8-8cb1-b15f2394e5ee",
          "name": "createPolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicyVersion?PolicyArn=PolicyArn&PolicyDocument=PolicyDocument&SetAsDefault=SetAsDefault",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new version of the specified managed policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d8ef8c8-adc0-4088-a737-0644cc0d26ee"
            }
          ]
        },
        {
          "id": "21c4f7d6-879e-411b-a2f3-db343fa69680",
          "name": "deletePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicy?PolicyArn=PolicyArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified managed policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a681a316-d7ad-4a9a-b739-fcd5b5efddcb"
            }
          ]
        },
        {
          "id": "253185cb-9195-4d5d-a631-8436d058a25f",
          "name": "deletePolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicyVersion?PolicyArn=PolicyArn&VersionId=VersionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified version from the specified managed policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ed74271-0f6f-4ce8-99b2-2a0b48fb1d61"
            }
          ]
        },
        {
          "id": "0a2517e0-1132-4dc6-81cd-393ba8120b83",
          "name": "getPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetPolicy?PolicyArn=PolicyArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the specified managed policy, including the policy's\n      default version and the total number of IAM users, groups, and roles to which the policy is\n      attached."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9667b918-bd4f-4fd5-8552-9fa96a363b8f"
            }
          ]
        },
        {
          "id": "4518614b-4bdd-4b69-aef9-ebf0e8bc0d5c",
          "name": "getPolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=GetPolicyVersion?PolicyArn=PolicyArn&VersionId=VersionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the specified version of the specified managed policy,\n      including the policy document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d8f6869-4352-4fbb-8821-70b6ed59bb90"
            }
          ]
        }
      ]
    },
    {
      "name": "Roles",
      "item": [
        {
          "id": "e7fbf373-751a-499c-a74c-4fb23846746d",
          "name": "createRole",
          "request": {
            "url": "http://example.com/api/?Action=CreateRole?AssumeRolePolicyDocument=AssumeRolePolicyDocument&Path=Path&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new role for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fec12a52-d028-43bf-baa5-092bf379989c"
            }
          ]
        },
        {
          "id": "1cef40a4-f1c0-4e50-861c-d55c9a051ab4",
          "name": "deleteRole",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRole?RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "794e955b-7c7d-4979-8745-bb528b225ca6"
            }
          ]
        },
        {
          "id": "a9eaac69-c0da-4d7b-9d58-d0cbb63bbecf",
          "name": "getRole",
          "request": {
            "url": "http://example.com/api/?Action=GetRole?RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the specified role, including the role's path, GUID, ARN,\n      and the role's trust policy that grants permission to assume the role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0de2240e-c852-4f6f-be12-fe98897148da"
            }
          ]
        },
        {
          "id": "698e1b6e-3885-41d3-942b-855500bb1961",
          "name": "listRoles",
          "request": {
            "url": "http://example.com/api/?Action=ListRoles?Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IAM roles that have the specified path prefix."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a801b7a7-bc74-4ee9-9ce3-6f42ad2c6812"
            }
          ]
        }
      ]
    },
    {
      "name": "SAML Providers",
      "item": [
        {
          "id": "8c8a3adc-191a-4991-bc72-16d0afcb002f",
          "name": "createSAMLProvider",
          "request": {
            "url": "http://example.com/api/?Action=CreateSAMLProvider?Name=Name&SAMLMetadataDocument=SAMLMetadataDocument",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an IAM resource that describes an identity provider (IdP) that supports SAML\n      2."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e123c36-603d-4a22-8d6b-c69669c58d0f"
            }
          ]
        },
        {
          "id": "e28d65f6-c667-4ce7-81b0-f9a5e2801492",
          "name": "deleteSAMLProvider",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSAMLProvider?SAMLProviderArn=SAMLProviderArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a SAML provider resource in IAM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbb97173-6d3d-4705-b66e-df860521460c"
            }
          ]
        },
        {
          "id": "6158f02d-afed-4142-9e96-529c6b1b09da",
          "name": "getSAMLProvider",
          "request": {
            "url": "http://example.com/api/?Action=GetSAMLProvider?SAMLProviderArn=SAMLProviderArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the SAML provider metadocument that was uploaded when the IAM SAML provider\n      resource object was created or updated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4aaa4da-a2ad-4b9b-9e79-fe6536f1b9ce"
            }
          ]
        },
        {
          "id": "a13ad188-979e-4f35-9931-25e7133f0843",
          "name": "listSAMLProviders",
          "request": {
            "url": "http://example.com/api/?Action=ListSAMLProviders?SAMLProviderList.member.N=SAMLProviderList.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the SAML provider resource objects defined in IAM in the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3411eae-f240-4f5d-a479-0d05b9dde30b"
            }
          ]
        }
      ]
    },
    {
      "name": "Service Specific Credentials",
      "item": [
        {
          "id": "cab36728-49b0-45c6-a8f0-bd7e1327d964",
          "name": "createServiceSpecificCredential",
          "request": {
            "url": "http://example.com/api/?Action=CreateServiceSpecificCredential?ServiceName=ServiceName&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates a set of credentials consisting of a user name and password that can be used\n      to access the service specified in the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "222c6d2e-d093-4643-9940-cc93f1cb618f"
            }
          ]
        },
        {
          "id": "d4e6c70a-9541-45ba-90f6-edc86cf6f74a",
          "name": "deleteServiceSpecificCredential",
          "request": {
            "url": "http://example.com/api/?Action=DeleteServiceSpecificCredential?ServiceSpecificCredentialId=ServiceSpecificCredentialId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified service-specific credential."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "347631bc-905e-45fb-a280-8e351b07b8f0"
            }
          ]
        },
        {
          "id": "b6d204f4-2b0e-42e0-b49f-ea5e0cc2fa9c",
          "name": "listServiceSpecificCredentials",
          "request": {
            "url": "http://example.com/api/?Action=ListServiceSpecificCredentials?ServiceName=ServiceName&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the service-specific credentials associated with the\n      specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21c408c2-3864-43ae-8a48-c22a75404800"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "fd985452-d580-4ad8-9287-fb610eadbdb0",
          "name": "createUser",
          "request": {
            "url": "http://example.com/api/?Action=CreateUser?Path=Path&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IAM user for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "904aff49-130b-40a2-9623-b8204fcd4e5f"
            }
          ]
        },
        {
          "id": "c85657cf-8e9b-408b-9457-ca78927145fb",
          "name": "deleteUser",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUser?UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b6d8bb2-1feb-4eb3-9aea-0c95084cb071"
            }
          ]
        },
        {
          "id": "0f7d0647-90af-4b43-bad0-3cb1f4795abb",
          "name": "getUser",
          "request": {
            "url": "http://example.com/api/?Action=GetUser?UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the specified IAM user, including the user's creation\n      date, path, unique ID, and ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccf281b0-f2db-49e7-b3fe-7cb0f6d3c202"
            }
          ]
        }
      ]
    },
    {
      "name": "Virtual MFA Device",
      "item": [
        {
          "id": "d1ef832d-0f3e-4007-8512-dc69b557a253",
          "name": "createVirtualMFADevice",
          "request": {
            "url": "http://example.com/api/?Action=CreateVirtualMFADevice?Path=Path&VirtualMFADeviceName=VirtualMFADeviceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new virtual MFA device for the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76fc1c8d-62a1-4aa3-9c6f-10d8b3a2c9f0"
            }
          ]
        },
        {
          "id": "8cd2776d-85b0-40b1-8e0f-0f61b876b233",
          "name": "deactivateMFADevice",
          "request": {
            "url": "http://example.com/api/?Action=DeactivateMFADevice?SerialNumber=SerialNumber&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates the specified MFA device and removes it from association with the user name\n      for which it was originally enabled."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75d12813-79d1-4ed9-a012-be1d35898e4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Password Policies",
      "item": [
        {
          "id": "ee2429ff-d247-4583-9d3e-a380f10b2959",
          "name": "deleteAccountPasswordPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAccountPasswordPolicy?LimitExceeded=LimitExceeded&NoSuchEntity=NoSuchEntity&ServiceFailure=ServiceFailure",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the password policy for the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c523aae9-4089-411b-ad6c-b0a8f3890d09"
            }
          ]
        }
      ]
    },
    {
      "name": "Server Certificates",
      "item": [
        {
          "id": "af9c157c-fe34-41b4-a1fd-2611fd1ab1a3",
          "name": "deleteServerCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteServerCertificate?ServerCertificateName=ServerCertificateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified server certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "104a7715-1372-4095-bbee-b95013f27a2f"
            }
          ]
        },
        {
          "id": "0f0545f0-f1b8-4cab-ba10-d478dcdf4e7f",
          "name": "getServerCertificate",
          "request": {
            "url": "http://example.com/api/?Action=GetServerCertificate?ServerCertificateName=ServerCertificateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the specified server certificate stored in IAM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7897f7c4-d3fa-4ac3-9f9b-2d11925772a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Signing Certificates",
      "item": [
        {
          "id": "da0fa01e-44c4-4a33-9ffb-567714c50305",
          "name": "deleteSigningCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSigningCertificate?CertificateId=CertificateId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a signing certificate associated with the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a42f00a-993f-41a8-9328-537ae7c1d217"
            }
          ]
        }
      ]
    },
    {
      "name": "SSH Public Key",
      "item": [
        {
          "id": "1538dd3b-8bf1-4e1e-918c-876432571530",
          "name": "deleteSSHPublicKey",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSSHPublicKey?SSHPublicKeyId=SSHPublicKeyId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified SSH public key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99d2dbd7-17a8-4153-83c4-c362d41e5b87"
            }
          ]
        },
        {
          "id": "68801ead-bc07-4c6a-a67b-d5ee0f90560e",
          "name": "getSSHPublicKey",
          "request": {
            "url": "http://example.com/api/?Action=GetSSHPublicKey?Encoding=Encoding&SSHPublicKeyId=SSHPublicKeyId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified SSH public key, including metadata about the key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "309cc16a-4023-48f4-b3cb-5fa85fab0a06"
            }
          ]
        }
      ]
    },
    {
      "name": "Virtual MFA Devices",
      "item": [
        {
          "id": "0f16bc74-c2f6-4a87-bd28-ef81e22a0bd2",
          "name": "deleteVirtualMFADevice",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVirtualMFADevice?SerialNumber=SerialNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a virtual MFA device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ea1a2a3-236a-486c-ab65-04797a22c1aa"
            }
          ]
        }
      ]
    },
    {
      "name": "MFA Devices",
      "item": [
        {
          "id": "d44b6ec7-010a-41b1-838f-abbacad53b5f",
          "name": "enableMFADevice",
          "request": {
            "url": "http://example.com/api/?Action=EnableMFADevice?AuthenticationCode1=AuthenticationCode1&AuthenticationCode2=AuthenticationCode2&SerialNumber=SerialNumber&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the specified MFA device and associates it with the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "595a1eae-bbe8-4c4b-a7a0-196e44769486"
            }
          ]
        },
        {
          "id": "1578d6b2-be6a-4fb7-a3e5-8b7b8ad71ebe",
          "name": "listMFADevices",
          "request": {
            "url": "http://example.com/api/?Action=ListMFADevices?Marker=Marker&MaxItems=MaxItems&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the MFA devices for an IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ffb64f0-4bc7-403d-b43c-53ddb68ab983"
            }
          ]
        }
      ]
    },
    {
      "name": "Credential Reports",
      "item": [
        {
          "id": "5f127dbc-cfdf-4ff8-8779-4e0c320ecca1",
          "name": "generateCredentialReport",
          "request": {
            "url": "http://example.com/api/?Action=GenerateCredentialReport?Description=Description&State=State",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates a credential report for the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6d91545-ae56-40bd-b0b2-ccac437f17eb"
            }
          ]
        },
        {
          "id": "aa39a421-a24e-4ff5-8b99-9b30c8afdb0a",
          "name": "getCredentialReport",
          "request": {
            "url": "http://example.com/api/?Action=GetCredentialReport?Content=Content&GeneratedTime=GeneratedTime&ReportFormat=ReportFormat",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a credential report for the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89ab5462-18a7-4fb8-a898-7056bb49c80a"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "a26897c1-05dc-414a-8277-e590f6642195",
          "name": "getAccountAuthorizationDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountAuthorizationDetails?Filter.member.N=Filter.member.N&Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about all IAM users, groups, roles, and policies in your AWS\n      account, including their relationships to one another."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5a76221-f62c-434b-a7eb-c416b9bb5e8b"
            }
          ]
        },
        {
          "id": "5aa69b1a-6114-41e6-9518-70f800ea505c",
          "name": "getAccountPasswordPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountPasswordPolicy?PasswordPolicy=PasswordPolicy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the password policy for the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a21a048a-3c1e-42c0-86b9-ff8aa217c225"
            }
          ]
        },
        {
          "id": "96098805-7113-4a9b-8770-9ca455954e21",
          "name": "getAccountSummary",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSummary?SummaryMap\n            , SummaryMap.entry.N.key (key), SummaryMapentry.N.value (value)=SummaryMap%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20SummaryMap.entry.N.key%20%28key%29%2C%20SummaryMapentry.N.value%20%28value%29",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about IAM entity usage and IAM quotas in the AWS\n      account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01f33e80-ffeb-46f3-afd3-5470d71bd4b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Context Keys For Custom Policies",
      "item": [
        {
          "id": "d3616ea1-4415-4099-9d1d-e1221d271f6b",
          "name": "getContextKeysForCustomPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetContextKeysForCustomPolicy?PolicyInputList.member.N=PolicyInputList.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of all of the context keys referenced in the input policies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b4e9e8a-a59c-45d2-9830-fdcf560c5116"
            }
          ]
        }
      ]
    },
    {
      "name": "Context Keys For Principal Policies",
      "item": [
        {
          "id": "f5fc1ba7-a043-4427-803a-48ebaf061722",
          "name": "getContextKeysForPrincipalPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetContextKeysForPrincipalPolicy?PolicyInputList.member.N=PolicyInputList.member.N&PolicySourceArn=PolicySourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of all of the context keys referenced in all of the IAM policies attached\n      to the specified IAM entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "911b7132-4d74-4613-8bf5-875fc949a026"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Aliases",
      "item": [
        {
          "id": "7300bb9e-356f-4436-9324-1ae52ae56a09",
          "name": "listAccountAliases",
          "request": {
            "url": "http://example.com/api/?Action=ListAccountAliases?Marker=Marker&MaxItems=MaxItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the account alias associated with the AWS account (Note: you can have only\n      one)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c92b07ad-0605-4ecd-8cc4-e91c3eec49cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Attached Group Policies",
      "item": [
        {
          "id": "11075dd5-397e-47a1-b3c3-1314215d3e46",
          "name": "listAttachedGroupPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListAttachedGroupPolicies?GroupName=GroupName&Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all managed policies that are attached to the specified IAM group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7f508fa-f675-4dfb-8293-27231493ae9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Attached Role Policies",
      "item": [
        {
          "id": "367f50d9-4615-402f-b252-8f1464e31412",
          "name": "listAttachedRolePolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListAttachedRolePolicies?Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all managed policies that are attached to the specified IAM role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d269d16e-807d-40ab-a700-ab47197835d4"
            }
          ]
        }
      ]
    },
    {
      "name": "Attached Use rPolicies",
      "item": [
        {
          "id": "6207a862-2288-4423-b2c3-403c6f3f3e29",
          "name": "listAttachedUserPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListAttachedUserPolicies?Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all managed policies that are attached to the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb8ca56b-b90f-40a7-9e69-342177083cc0"
            }
          ]
        }
      ]
    },
    {
      "name": "Entities For Policies",
      "item": [
        {
          "id": "d6432414-06e0-4e79-8459-baa4cf065201",
          "name": "listEntitiesForPolicy",
          "request": {
            "url": "http://example.com/api/?Action=ListEntitiesForPolicy?EntityFilter=EntityFilter&Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix&PolicyArn=PolicyArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all IAM users, groups, and roles that the specified managed policy is attached\n      to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35d94681-ec36-435b-ae2b-8927e489881d"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups For User",
      "item": [
        {
          "id": "70e4af4e-591b-4d13-904e-1fa3c30aecc8",
          "name": "listGroupsForUser",
          "request": {
            "url": "http://example.com/api/?Action=ListGroupsForUser?Marker=Marker&MaxItems=MaxItems&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IAM groups that the specified IAM user belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1b95129-69b3-4694-a575-79f72d989c00"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance Profiles For Role",
      "item": [
        {
          "id": "d0e3f839-c37c-4e33-9897-a2d3cb19336b",
          "name": "listInstanceProfilesForRole",
          "request": {
            "url": "http://example.com/api/?Action=ListInstanceProfilesForRole?Marker=Marker&MaxItems=MaxItems&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the instance profiles that have the specified associated IAM role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "551e9fa1-6824-4e43-bdf2-4492815b4488"
            }
          ]
        }
      ]
    },
    {
      "name": "listPolicies",
      "item": [
        {
          "id": "54b389aa-2d4b-434e-8452-ea8cc1093003",
          "name": "listPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListPolicies?Marker=Marker&MaxItems=MaxItems&OnlyAttached=OnlyAttached&PathPrefix=PathPrefix&Scope=Scope",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the managed policies that are available in your AWS account, including your\n      own customer-defined managed policies and all AWS managed policies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a8d2ef0-697b-4a24-bd43-3988ddccaf4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Policy Versions",
      "item": [
        {
          "id": "be1f099e-d440-4f05-8e88-26a1515789b0",
          "name": "listPolicyVersions",
          "request": {
            "url": "http://example.com/api/?Action=ListPolicyVersions?Marker=Marker&MaxItems=MaxItems&PolicyArn=PolicyArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists information about the versions of the specified managed policy, including the\n      version that is currently set as the policy's default version."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62620005-0773-4fa2-b1de-3b0d76a8b758"
            }
          ]
        }
      ]
    },
    {
      "name": "Serve rCertificates",
      "item": [
        {
          "id": "05807f2e-22a5-43a9-ae76-6dd09396ae33",
          "name": "listServerCertificates",
          "request": {
            "url": "http://example.com/api/?Action=ListServerCertificates?Marker=Marker&MaxItems=MaxItems&PathPrefix=PathPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the server certificates stored in IAM that have the specified path prefix."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0753cdc2-7b73-4446-ad0c-02784c07c6da"
            }
          ]
   