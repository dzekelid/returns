swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 1
info:
  title: Capital One DevExchange
  description: nessie-is-capital-ones-hackathon-api-that-gives-you-access-to-a-multitude-of-real-publicfacing-data--such-as-atm-and-bank-branch-locations--along-with-mock-customer-account-data--use-http-requests-to-set-up-peertopeer-transactions-simulate-a-weekly-paycheck-or-even-schedule-bills-for-customers-this-is-all-structured-in-a-way-that-resembles-how-we-actually-run-things-here-at-capital-one-
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
  /accounts/{id}/bills:
    get:
      summary: Get all bills for a specific account
      description: Returns the bills that are tied to the specific account.
      operationId: returns-the-bills-that-are-tied-to-the-specific-account
      x-api-path-slug: accountsidbills-get
      parameters:
      - in: path
        name: id
        description: ID of account to fetch bills for
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Bills
  /accounts/{id}/customer:
    get:
      summary: Get customer that owns the specified account
      description: Returns the customer that the account belongs to.
      operationId: returns-the-customer-that-the-account-belongs-to
      x-api-path-slug: accountsidcustomer-get
      parameters:
      - in: path
        name: id
        description: ID of customer that account will belong to
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Customer
  /accounts/{id}/deposits:
    get:
      summary: Get all deposits
      description: Returns the deposits that you are involved in.
      operationId: returns-the-deposits-that-you-are-involved-in
      x-api-path-slug: accountsiddeposits-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the deposit
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Deposits
  /accounts/{id}/loans:
    get:
      summary: Get all loans
      description: Returns the loans that you are involved in.
      operationId: returns-the-loans-that-you-are-involved-in
      x-api-path-slug: accountsidloans-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the loan
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Loans
  /accounts/{id}/purchases:
    get:
      summary: Get all purchases
      description: Returns the purchases that you are involved in.
      operationId: returns-the-purchases-that-you-are-involved-in
      x-api-path-slug: accountsidpurchases-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the purchase
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Purchases
  /accounts/{id}/transfers:
    get:
      summary: Get all transfers
      description: Returns the transfers that you are involved in.
      operationId: returns-the-transfers-that-you-are-involved-in
      x-api-path-slug: accountsidtransfers-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the transfer
      - in: query
        name: type
        description: When param is empty, will return transfers associated with account
          where account is payer AND payee
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Transfers
  /accounts/{id}/withdrawals:
    get:
      summary: Get all withdrawals
      description: Returns the withdrawals that you are involved in.
      operationId: returns-the-withdrawals-that-you-are-involved-in
      x-api-path-slug: accountsidwithdrawals-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the withdrawal
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Withdrawals