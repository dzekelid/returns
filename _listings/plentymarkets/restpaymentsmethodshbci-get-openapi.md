---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Returns the HBCI-Account count
  description: Returns the hbci-account count.
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