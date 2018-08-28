swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 1
info:
  title: Azure Blockchain Workbench REST API
  description: the-azure-blockchain-workbench-rest-api-is-a-workbench-extensibility-point-which-allows-developers-to-create-and-manage-blockchain-applications-manage-users-and-organizations-within-a-consortium-integrate-blockchain-applications-into-services-and-platforms-perform-transactions-on-a-blockchain-and-retrieve-transactional-and-contract-data-from-a-blockchain-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/health:
    get:
      summary: Get Api Health
      description: |-
        Returns the health of the system. See https://docs.microsoft.com/en-us/azure/architecture/patterns/health-endpoint-monitoring
                     for more details.
      operationId: Health
      x-api-path-slug: apihealth-get
      responses:
        200:
          description: OK
      tags:
      - Api
      - Health
  /api/v1/users/me:
    get:
      summary: Get Users Me
      description: Returns the current user.
      operationId: MeGet
      x-api-path-slug: apiv1usersme-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me