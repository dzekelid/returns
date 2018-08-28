---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Get Queue Members
  description: Returns the list of members in the queue identified by {QueueSid}.
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
  /Accounts/{AccountSid}/ConnectApps.{format}:
    get:
      summary: Get Connected Apps
      description: Returns a list of Connect App resource representations, each representingna
        Connect App in your account. The list includes paging information.n
      operationId: returns-a-list-of-connect-app-resource-representations-each-representinga-connect-app-in-your-accoun
      x-api-path-slug: accountsaccountsidconnectapps-format-get
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
  /Accounts/{AccountSid}/IncomingPhoneNumbers/Local.{format}:
    get:
      summary: Get Incoming Local Phone Numbers
      description: Returns a list of local <IncomingPhoneNumber> elements, each representing
        a local (not toll-free) phone number given to your account, under an <IncomingPhoneNumbers>
        list element that includes paging information. Works exactly the same as the
        IncomingPhoneNumber resource, but filters out toll-free numbers.
      operationId: returns-a-list-of-local-incomingphonenumber-elements-each-representing-a-local-not-tollfree-phone-nu
      x-api-path-slug: accountsaccountsidincomingphonenumberslocal-format-get
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
      - Incoming Phone Numbers
  /Accounts/{AccountSid}/IncomingPhoneNumbers/Mobile.{format}:
    get:
      summary: Get Incoming Phone Numbers
      description: Returns a list of local <IncomingPhoneNumber> elements, each representing
        a mobile phone number given to your account, under an <IncomingPhoneNumbers>
        list element that includes paging information. Works exactly the same as the
        IncomingPhoneNumber resource, but filters out local and toll free numbers.
      operationId: returns-a-list-of-local-incomingphonenumber-elements-each-representing-a-mobile-phone-number-given-t
      x-api-path-slug: accountsaccountsidincomingphonenumbersmobile-format-get
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
      - Incoming Phone Numbers
  /Accounts/{AccountSid}/Messages.{format}:
    get:
      summary: Get Message Media
      description: Returns a list of messages associated with your account. The list
        includes paging information.
      operationId: returns-a-list-of-messages-associated-with-your-account-the-list-includes-paging-information
      x-api-path-slug: accountsaccountsidmessages-format-get
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
      - Messages
  /Accounts/{AccountSid}/Messages/{MessageSid}:
    get:
      summary: Get Message Media
      description: Returns a single message specified by the provided {MessageSid}.n
      operationId: returns-a-single-message-specified-by-the-provided-messagesid
      x-api-path-slug: accountsaccountsidmessagesmessagesid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: MessageSid
        description: A 34 character string that uniquely identifies the message
      responses:
        200:
          description: OK
      tags:
      - Messages
  /Accounts/{AccountSid}/Messages/{MessageSid}/Media:
    get:
      summary: Get Message Media
      description: Returns a list of media associated with your message.
      operationId: returns-a-list-of-media-associated-with-your-message
      x-api-path-slug: accountsaccountsidmessagesmessagesidmedia-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: MessageSid
        description: A 34 character string that uniquely identifies the message
      responses:
        200:
          description: OK
      tags:
      - Messages
  /Accounts/{AccountSid}/OutgoingCallerIds:
    get:
      summary: Get Outgoing Caller Ids
      description: Returns a list of OutgoingCallerId resource representations, each
        representingna Caller ID number valid for an account. The list includes paging
        information.n
      operationId: returns-a-list-of-outgoingcallerid-resource-representations-each-representinga-caller-id-number-vali
      x-api-path-slug: accountsaccountsidoutgoingcallerids-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Outgoing Caller IDs
  /Accounts/{AccountSid}/Queues:
    get:
      summary: Get Queues
      description: Returns a list of queues within an account. The list includes pagingninformation.n
      operationId: returns-a-list-of-queues-within-an-account-the-list-includes-paginginformation
      x-api-path-slug: accountsaccountsidqueues-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Queues
  /Accounts/{AccountSid}/Queues/{QueueSid}/Members:
    get:
      summary: Get Queue Members
      description: Returns the list of members in the queue identified by {QueueSid}.
      operationId: returns-the-list-of-members-in-the-queue-identified-by-queuesid
      x-api-path-slug: accountsaccountsidqueuesqueuesidmembers-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
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