---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Get Remote Access Session
  version: 1.0.0
  description: Returns a link to a currently running remote access session.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetAccountSettings:
    get:
      summary: Get Account Settings
      description: Returns the number of unmetered iOS and/or unmetered Android devices
        that have been purchased by the account.
      operationId: getAccountSettings
      x-api-path-slug: actiongetaccountsettings-get
      parameters:
      - in: query
        name: accountSettings
        description: A container for account-level settings within AWS Device Farm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Settings
  /?Action=GetRemoteAccessSession:
    get:
      summary: Get Remote Access Session
      description: Returns a link to a currently running remote access session.
      operationId: getRemoteAccessSession
      x-api-path-slug: actiongetremoteaccesssession-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the remote access session about
          which you want to get session information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
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