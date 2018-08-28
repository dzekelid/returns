swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/contacts/{email}/files:
    get:
      summary: Get Accounts Contacts Email Files
      description: Lists files exchanged with a contact. Returns the latest attachments
        exchanged with one or more email addresses. By "exchanged with Mr. X" we mean
        any file attached to an email received from Mr. X, sent to Mr. X or sent by
        anyone to both Mr. X and the mailbox owner.
      operationId: listAccountContactFiles_
      x-api-path-slug: accountsidcontactsemailfiles-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Files
  /accounts/{id}/contacts/{email}/messages:
    get:
      summary: Get Accounts Contacts Email Messages
      description: Lists messages where a contact is present. Returns the latest email
        messages exchanged with one or more email addresses. By "exchanged with Mr.
        X" we mean any email received from Mr. X, sent to Mr. X or sent by anyone
        to both Mr. X and the mailbox owner.
      operationId: listAccountContactMessages_
      x-api-path-slug: accountsidcontactsemailmessages-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Messages
  /accounts/{id}/contacts/{email}/threads:
    get:
      summary: Get Accounts Contacts Email Threads
      description: Lists threads where a contact is present. Returns the latest email
        threads exchanged with one or more email addresses. By "exchanged with Mr.
        X" we mean any email received from Mr. X, sent to Mr. X or sent by anyone
        to both Mr. X and the mailbox owner.
      operationId: listAccountContactThreads_
      x-api-path-slug: accountsidcontactsemailthreads-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Threads
  /accounts/{id}/files/{fileId}/content:
    get:
      summary: Get Accounts Files Fileid Content
      description: 'Downloads a given file. Returns the content a given attachment.
        On-demand data retrieval: since we do not keep full copies of attachments
        on our servers, the file has to be retrieved from the IMAP server when this
        call is made. If the IMAP server is unreachable at the time the call is made,
        this call will return an error.'
      operationId: getAccountFileContent_
      x-api-path-slug: accountsidfilesfileidcontent-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Content
  /accounts/{id}/files/{fileId}/related:
    get:
      summary: Get Accounts Files Fileid Related
      description: Lists other files related to a given file. Returns a list of files
        that are related to the given file. Currently, relation between files is based
        on how similar their names are.
      operationId: listAccountFileRelatedFiles_
      x-api-path-slug: accountsidfilesfileidrelated-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Related
  /accounts/{id}/files/{fileId}/revisions:
    get:
      summary: Get Accounts Files Fileid Revisions
      description: Lists other revisions of a given file. Returns a list of revisions
        attached to other emails in the mailbox for a given file. Two files are considered
        revisions of the same document if their file names are identical outside of
        revision indicators such as dates, author initials, version numbers and keywords
        like "final" or "draft".
      operationId: listAccountFileRevisions_
      x-api-path-slug: accountsidfilesfileidrevisions-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Revisions
  /accounts/{id}/messages/{message_id}/source:
    get:
      summary: Get Accounts Messages Message Source
      description: 'Fetches the message source. Returns the raw RFC-822 message source
        for the message (including attachments) with no parsing or decoding to any
        portions of the message. On-demand data retrieval: since we do not keep full
        copies of emails on our servers, this call triggers a connection to the IMAP
        server to fetch the message. Attachments are part of the message source so
        they will impact how fast this call responds.'
      operationId: getAccountMessageSource_
      x-api-path-slug: accountsidmessagesmessage-idsource-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Source
  /accounts/{id}/sources/{label}/folders:
    get:
      summary: Get Accounts Sources Label Folders
      description: Lists folders in an IMAP source. Returns folders existing in a
        given IMAP account.
      operationId: listAccountSourceFolders_
      x-api-path-slug: accountsidsourceslabelfolders-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Folders
  /accounts/{id}/sources/{label}/sync:
    get:
      summary: Get Accounts Sources Label Sync
      description: Gets the sync status of a data source. Returns the timestamps for
        the last time the source has been synced with the origin mailbox.
      operationId: getAccountSourceSyncStatus_
      x-api-path-slug: accountsidsourceslabelsync-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Sync
  /accounts/{id}/sync:
    get:
      summary: Get Accounts Sync
      description: Gets the sync status for all sources of the account. Returns the
        timestamps for the last time a source has been synced with the origin mailbox.
      operationId: getAllAccountSourcesSyncStatus_
      x-api-path-slug: accountsidsync-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sync
  /accounts/{id}/threads/{thread_id}:
    get:
      summary: Get Accounts Threads Thread
      description: |-
        Returns files, contacts and messages on a given thread. The purpose is to allow Gmail extensions to easily retrieve data when users's load a conversation in the Gmail UI. Hence, threads are identified by the value of their Gmail thread prefixed with "gm-".
        For example, if the URL of a conversation in the Gmail UI is https://mail.google.com/mail/u/0/#mbox/13119ab37f00b826, you would obtain the details about this thread by calling:
        GET https://api.context.io/2.0/accounts/<accountId>/threads/gm-13119ab37f00b826

        What about threads on non-Gmail mailboxes?
        You can retrieve thread information for any message using the Thread resource of that message.
      operationId: getAccountThread_
      x-api-path-slug: accountsidthreadsthread-id-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: thread_id
        description: A gmail_thread_id prefixed with gm-
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Threads
      - Thread