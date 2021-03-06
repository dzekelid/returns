---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get return policy
  description: Get return policy for given ID.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/customer_contracts/{contractId}:
    get:
      summary: Returns a single contract
      description: Returns a single contract.
      operationId: getRestCustomerContractsContract
      x-api-path-slug: restcustomer-contractscontractid-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Single
      - Contract
  /rest/customer_contracts/{contractId}/sign:
    get:
      summary: Returns signing of a contract
      description: Returns signing of a contract.
      operationId: getRestCustomerContractsContractSign
      x-api-path-slug: restcustomer-contractscontractidsign-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Signing
      - Of
      - Contract
  /rest/payments/methods/hbci:
    get:
      summary: Returns the HBCI-Account count
      description: Returns the hbci-account count.
      operationId: getRestPaymentsMethodsHbci
      x-api-path-slug: restpaymentsmethodshbci-get
      responses:
        200:
          description: OK
      tags:
      - Returns
      - HBCI-Account
      - Count
  /rest/accounts/contacts/{contactId}/related_data:
    get:
      summary: Return all contact related data
      description: Returns all contact related data.
      operationId: getRestAccountsContactsContactRelatedData
      x-api-path-slug: restaccountscontactscontactidrelated-data-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Contact
      - Related
      - Data
  /rest/markets/ebay/return_policies/{id}:
    get:
      summary: Get return policy
      description: Get return policy for given ID.
      operationId: getRestMarketsEbayReturnPolicies
      x-api-path-slug: restmarketsebayreturn-policiesid-get
      parameters:
      - in: query
        name: credentialsId
        description: The ID of credentials for which to get the policy
      - in: path
        name: id
      - in: query
        name: marketplaceId
        description: The ID of the marketplace for which to get the policy
      responses:
        200:
          description: OK
      tags:
      - Return
      - Policy
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