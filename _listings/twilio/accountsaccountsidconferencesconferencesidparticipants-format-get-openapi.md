---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Get Conference Call Participants
  description: Returns the list of participants in the conference identified byn{ConferenceSid}.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/AuthorizedConnectApps.{format}:
    get:
      summary: Get Authorized Connected Apps
      description: Returns a list of Connect App resource representations, each representing
        anConnect App youve authorized to access your account. The list includesnpaging
        information.n
      operationId: returns-a-list-of-connect-app-resource-representations-each-representing-aconnect-app-youve-authoriz
      x-api-path-slug: accountsaccountsidauthorizedconnectapps-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /Accounts/{AccountSid}/AvailablePhoneNumbers/{IsoCountryCode}/Local.{format}:
    get:
      summary: Get Available Local Phone Numbers
      description: Returns a list of local AvailablePhoneNumber resource representationsnthat
        match the specified filters, each representing a phone number thanis currently
        available for provisioning within your account.n
      operationId: returns-a-list-of-local-availablephonenumber-resource-representationsthat-match-the-specified-filter
      x-api-path-slug: accountsaccountsidavailablephonenumbersisocountrycodelocal-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IsoCountryCode
        description: ISO 3166-1 alpha-2
      responses:
        200:
          description: OK
      tags:
      - Phone Numbers
  /Accounts/{AccountSid}/AvailablePhoneNumbers/{IsoCountryCode}/Mobile.{format}:
    get:
      summary: Get Available Mobile Phone Numbers
      description: Returns a list of mobile AvailablePhoneNumber resource representations
        that match the specified filters, each representing a phone number that is
        currently available for provisioning within your account.
      operationId: returns-a-list-of-mobile-availablephonenumber-resource-representations-that-match-the-specified-filt
      x-api-path-slug: accountsaccountsidavailablephonenumbersisocountrycodemobile-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IsoCountryCode
        description: ISO 3166-1 alpha-2
      responses:
        200:
          description: OK
      tags:
      - Phone Numbers
  /Accounts/{AccountSid}/AvailablePhoneNumbers/{IsoCountryCode}/TollFree.{format}:
    get:
      summary: Get Available Toll Free Phone Numbers
      description: Returns a list of toll-free AvailablePhoneNumber elements that
        match thenspecified filters, each representing a phone number that is currentlynavailable
        for provisioning within your account. To provision an availablenphone number,
        POST the number to the IncomingPhoneNumbers resource.n
      operationId: returns-a-list-of-tollfree-availablephonenumber-elements-that-match-thespecified-filters-each-repres
      x-api-path-slug: accountsaccountsidavailablephonenumbersisocountrycodetollfree-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IsoCountryCode
        description: ISO 3166-1 alpha-2
      responses:
        200:
          description: OK
      tags:
      - Phone Numbers
  /Accounts/{AccountSid}/Calls/{CallSid}/Recordings.{format}:
    get:
      summary: Get Recordings
      description: Returns a list of Recording resource representations, each representing
        anrecording generated during the course of a phone call.n
      operationId: returns-a-list-of-recording-resource-representations-each-representing-arecording-generated-during-t
      x-api-path-slug: accountsaccountsidcallscallsidrecordings-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CallSid
        description: A 34 character string that uniquely identifies the call
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Recordings
  /Accounts/{AccountSid}/Conferences.{format}:
    get:
      summary: Get Conference Calls
      description: Returns a list of conferences within an account. The list includes
        pagingninformation.n
      operationId: returns-a-list-of-conferences-within-an-account-the-list-includes-paginginformation
      x-api-path-slug: accountsaccountsidconferences-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Conference Calls
  /Accounts/{AccountSid}/Conferences/{ConferenceSid}/Participants.{format}:
    get:
      summary: Get Conference Call Participants
      description: Returns the list of participants in the conference identified byn{ConferenceSid}.n
      operationId: returns-the-list-of-participants-in-the-conference-identified-byconferencesid
      x-api-path-slug: accountsaccountsidconferencesconferencesidparticipants-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: ConferenceSid
        description: A 34 character string that uniquely identifies the conference
          call object
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Conference Calls
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---