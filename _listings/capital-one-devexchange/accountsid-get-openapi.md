---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 0
info:
  title: Capital One DevExchange Get account by id
  description: Returns the account with the specific id
  version: 1.0.0
host: api.reimaginebanking.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: Get all accounts
      description: Returns the accounts that have been assigned to you.
      operationId: returns-the-accounts-that-have-been-assigned-to-you
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: type
        description: Empty Param will return all types of accounts
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
  /accounts/{id}:
    get:
      summary: Get account by id
      description: Returns the account with the specific id
      operationId: returns-the-account-with-the-specific-id
      x-api-path-slug: accountsid-get
      parameters:
      - in: path
        name: id
        description: ID of account that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
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