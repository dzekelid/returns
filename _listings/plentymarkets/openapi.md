swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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