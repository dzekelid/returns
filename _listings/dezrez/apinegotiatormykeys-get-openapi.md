---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Return all Negotiator keys for the side bar display.
  version: 1.0.0
  description: Return all negotiator keys for the side bar display..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/agency/teams:
    get:
      summary: Returns a list of team groups for the agency.
      description: Returns a list of team groups for the agency..
      operationId: Agency_TeamsBypageSizeBypageNumberByteamType
      x-api-path-slug: apiagencyteams-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Team
      - Groupsthe
      - Agency
  /api/analytics/campaigns:
    get:
      summary: returns a list of all of the campaigns for an agency
      description: Returns a list of all of the campaigns for an agency.
      operationId: Analytics_GetCampaigns
      x-api-path-slug: apianalyticscampaigns-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - ""
      - Of
      - Campaignsan
      - Agency
  /api/appointment/freebusy:
    post:
      summary: Returns Free/Busy information regarding multiple people.
      description: Returns free/busy information regarding multiple people..
      operationId: Appointment_GetFreeBusyByquery
      x-api-path-slug: apiappointmentfreebusy-post
      parameters:
      - in: body
        name: query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Free
      - Busy
      - Information
      - Regarding
      - Multiple
      - People
  /api/customtextdescription/distinctcustompropertydescriptions:
    get:
      summary: Returns a list of the distinct defined custom descriptions for a property
      description: Returns a list of the distinct defined custom descriptions for
        a property.
      operationId: CustomTextDescription_DistinctCustomPropertyDescriptions
      x-api-path-slug: apicustomtextdescriptiondistinctcustompropertydescriptions-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Distinct
      - Defined
      - Custom
      - Descriptionsa
      - Property
  /api/todo/gettodonotes:
    get:
      summary: Returns all notes for todo
      description: Returns all notes for todo.
      operationId: DefaultToDo_GetTodoNotesBytodoId
      x-api-path-slug: apitodogettodonotes-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: todoId
      responses:
        200:
          description: OK
      tags:
      - Returns
      - ""
      - Notestodo
  /api/documentgeneration/metadata/{major}/{minor}/{build}/{revision}:
    get:
      summary: Returns the data contract to configure the word plugin for creating
        templates
      description: Returns the data contract to configure the word plugin for creating
        templates.
      operationId: DocumentGeneration_GetLetterEditorDataContractBymajorByminorBybuildByrevision
      x-api-path-slug: apidocumentgenerationmetadatamajorminorbuildrevision-get
      parameters:
      - in: path
        name: build
      - in: path
        name: major
      - in: path
        name: minor
      - in: path
        name: revision
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Data
      - Contract
      - To
      - Configure
      - Word
      - Plugincreating
      - Templates
  /api/documentgeneration/lettertemplate/{letterTemplateId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetLetterTemplateByletterTemplateId
      x-api-path-slug: apidocumentgenerationlettertemplatelettertemplateid-get
      parameters:
      - in: path
        name: letterTemplateId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/mergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetPrintableMergeTemplates
      x-api-path-slug: apidocumentgenerationmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/unusedmergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency that are
        not currently used in any envelope templates
      description: Returns a list of lettertemplates associated to this agency that
        are not currently used in any envelope templates.
      operationId: DocumentGeneration_GetUnusedMergeTemplates
      x-api-path-slug: apidocumentgenerationunusedmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - That
      - Are
      - Not
      - Currently
      - Used
      - In
      - Any
      - Envelope
      - Templates
  /api/documentgeneration/templatesusinganalytics/{analyticsId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency and to
        a particular google analyitics campaign
      description: Returns a list of lettertemplates associated to this agency and
        to a particular google analyitics campaign.
      operationId: DocumentGeneration_GetTemplatesUsingAnalyticsByanalyticsId
      x-api-path-slug: apidocumentgenerationtemplatesusinganalyticsanalyticsid-get
      parameters:
      - in: path
        name: analyticsId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - To
      - Particular
      - Google
      - Analyitics
      - Campaign
  /api/documentgeneration/bagcontent:
    get:
      summary: Returns the detail of the sack of correspondence that has just been
        prepared
      description: Returns the detail of the sack of correspondence that has just
        been prepared.
      operationId: DocumentGeneration_GetBagContent
      x-api-path-slug: apidocumentgenerationbagcontent-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Detail
      - Of
      - Sack
      - Of
      - Correspondence
      - That
      - Has
      - Just
      - Been
      - Prepared
  /api/documentgeneration/sackcontent/{sackReference}:
    get:
      summary: Returns the detail of the all outstanding sacks
      description: Returns the detail of the all outstanding sacks.
      operationId: DocumentGeneration_GetSackContentBysackReference
      x-api-path-slug: apidocumentgenerationsackcontentsackreference-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Detail
      - Of
      - ""
      - Outstanding
      - Sacks
  /api/documentgeneration/insertabletemplates:
    get:
      summary: Returns a list of insertable templates associated to this agency
      description: Returns a list of insertable templates associated to this agency.
      operationId: DocumentGeneration_GetPrintableInsertableTemplates
      x-api-path-slug: apidocumentgenerationinsertabletemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Insertable
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/headertemplates:
    get:
      summary: Returns a list of header templates associated to this agency with their
        associated brand info
      description: Returns a list of header templates associated to this agency with
        their associated brand info.
      operationId: DocumentGeneration_GetPrintableHeaderTemplates
      x-api-path-slug: apidocumentgenerationheadertemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Header
      - Templates
      - Associated
      - To
      - This
      - Agency
      - Their
      - Associated
      - Brand
      - Info
  /api/documentgeneration/envelopetemplates:
    get:
      summary: Returns a list of envelope templates associated to this agency
      description: Returns a list of envelope templates associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplates
      x-api-path-slug: apidocumentgenerationenvelopetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplate/{id}:
    get:
      summary: Returns a envelope template
      description: Returns a envelope template.
      operationId: DocumentGeneration_GetEnvelopeTemplateByid
      x-api-path-slug: apidocumentgenerationenvelopetemplateid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Envelope
      - Template
  /api/documentgeneration/envelopetemplatepack/{id}:
    get:
      summary: Returns a envelope template pack
      description: Returns a envelope template pack.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackByid
      x-api-path-slug: apidocumentgenerationenvelopetemplatepackid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Envelope
      - Template
      - Pack
  /api/documentgeneration/envelopetemplatepacks:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePacks
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacktypes:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackTypesByinUseOnly
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacktypes-get
      parameters:
      - in: query
        name: inUseOnly
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/emailtemplates:
    get:
      summary: Returns a list of email templates associated to this agency
      description: Returns a list of email templates associated to this agency.
      operationId: DocumentGeneration_GetEmailTemplates
      x-api-path-slug: apidocumentgenerationemailtemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Email
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/templates/{templateType}:
    get:
      summary: Returns a list of mergable templates for any type associated to this
        agency
      description: Returns a list of mergable templates for any type associated to
        this agency.
      operationId: DocumentGeneration_GetTemplatesBytemplateType
      x-api-path-slug: apidocumentgenerationtemplatestemplatetype-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: templateType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Mergable
      - Templatesany
      - Type
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/smstemplates:
    get:
      summary: Returns a list of sms templates associated to this agency
      description: Returns a list of sms templates associated to this agency.
      operationId: DocumentGeneration_GetSmsTemplates
      x-api-path-slug: apidocumentgenerationsmstemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Sms
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/enum:
    get:
      summary: "Returns a list of possible values for an enum if you just specify
        {typeName}.\r\nReturns a an enum if you specify {typeName} and {systemName}."
      description: "Returns a list of possible values for an enum if you just specify
        {typename}.\r\nreturns a an enum if you specify {typename} and {systemname}.."
      operationId: Enum_GetBytypeNameBysystemNameByeventCategoryType
      x-api-path-slug: apienum-get
      parameters:
      - in: query
        name: eventCategoryType
        description: Where the enum has values which are categorised, this filters
          on that category
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: systemName
        description: The system name of the enum to get
      - in: query
        name: typeName
        description: The type of enum to get
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Possible
      - Valuesan
      - Enum
      - If
      - You
      - Just
      - Specify
      - TypeName
      - Returns
      - Enum
      - If
      - You
      - Specify
      - TypeName
      - SystemName
  /api/ExternalProvider:
    get:
      summary: Returns a URL that will start the process of authorisation with the
        external provider - normally using the OAuth1/2 protocol suite.
      description: Returns a url that will start the process of authorisation with
        the external provider - normally using the oauth1/2 protocol suite..
      operationId: ExternalProvider_GetAuthoriseAgencyUrlByexternalProviderId
      x-api-path-slug: apiexternalprovider-get
      parameters:
      - in: query
        name: externalProviderId
        description: The external provider identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - URL
      - That
      - Will
      - Start
      - Process
      - Of
      - Authorisation
      - External
      - Provider
      - '-'
      - Normally
      - Using
      - OAuth1
      - "2"
      - Protocol
      - Suite
  /api/group/matches/find:
    post:
      summary: Returns property matches using their Id
      description: Returns property matches using their id.
      operationId: Group_FindMatchesByqueryDataContract
      x-api-path-slug: apigroupmatchesfind-post
      parameters:
      - in: body
        name: queryDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Matches
      - Using
      - Their
      - Id
  /api/group/{id}/getpropertyroleidsalreadysent:
    get:
      summary: returns a list of the property role ids that should be excluded from
        mailouts to this role id because the have been sent before
      description: Returns a list of the property role ids that should be excluded
        from mailouts to this role id because the have been sent before.
      operationId: Group_GetPropertyMarketingRoleIdsSentByidBywithinDaysByresendPriceChangedProperties
      x-api-path-slug: apigroupidgetpropertyroleidsalreadysent-get
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: query
        name: resendPriceChangedProperties
        description: include the properties that have had to a price change or withdrawn
          event since it was last sent to them
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: withinDays
        description: number of days since the last time it was sent, send 0 for all
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Property
      - Role
      - Ids
      - That
      - Should
      - Be
      - Excluded
      - From
      - Mailouts
      - To
      - This
      - Role
      - Id
      - Because
      - Have
      - Been
      - Sent
      - Before
  /api/group/geoaggregation/{zoom}:
    post:
      summary: Returns GeoAggregations of all searching groups
      description: Returns geoaggregations of all searching groups.
      operationId: Group_GeoAggregationByzoom
      x-api-path-slug: apigroupgeoaggregationzoom-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: zoom
      responses:
        200:
          description: OK
      tags:
      - Returns
      - GeoAggregations
      - Of
      - ""
      - Searching
      - Groups
  /api/locale/{culture}:
    get:
      summary: returns the json file containing localization for the app based on
        a culture string, and any custom values for the agent
      description: Returns the json file containing localization for the app based
        on a culture string, and any custom values for the agent.
      operationId: Locale_GetLocalisationFileByculture
      x-api-path-slug: apilocaleculture-get
      parameters:
      - in: path
        name: culture
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Json
      - File
      - Containing
      - Localizationthe
      - App
      - Based
      - "On"
      - Culture
      - String
      - ""
      - Any
      - Custom
      - Valuesthe
      - Agent
  /api/negotiator/my/groups/favourite:
    get:
      summary: Returns a list of the logged in negotiators favourite groups.
      description: Returns a list of the logged in negotiators favourite groups..
      operationId: Negotiator_FavouriteGroupsBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormygroupsfavourite-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Logged
      - In
      - Negotiators
      - Favourite
      - Groups
  /api/people/findbyemail:
    get:
      summary: Returns a list of people that have the supplied email address.
      description: Returns a list of people that have the supplied email address..
      operationId: People_GetPeopleWithEmailAddressByemailAddress
      x-api-path-slug: apipeoplefindbyemail-get
      parameters:
      - in: query
        name: emailAddress
        description: The email address
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - People
      - That
      - Have
      - Supplied
      - Email
      - Address
  /api/property/geoaggregation/{zoom}:
    post:
      summary: Returns GeoAggregations of all properties
      description: Returns geoaggregations of all properties.
      operationId: Property_GeoAggregationByzoom
      x-api-path-slug: apipropertygeoaggregationzoom-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: zoom
      responses:
        200:
          description: OK
      tags:
      - Returns
      - GeoAggregations
      - Of
      - ""
      - Properties
  /api/region/favourites:
    get:
      summary: Returns favorite regions
      description: Returns favorite regions.
      operationId: Region_GetAllFavourites
      x-api-path-slug: apiregionfavourites-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Favorite
      - Regions
  /api/region/favourites/{favouriteRegionId}:
    get:
      summary: Returns favorite regions
      description: Returns favorite regions.
      operationId: Region_GetFavouriteByfavouriteRegionId
      x-api-path-slug: apiregionfavouritesfavouriteregionid-get
      parameters:
      - in: path
        name: favouriteRegionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Favorite
      - Regions
  /api/teamsecurity/permissionsforgroup:
    get:
      summary: This returns security permissions that a group has on other groups
      description: This returns security permissions that a group has on other groups.
      operationId: TeamGroupSecurity_GetSecurityPermissionsForGroupByteamId
      x-api-path-slug: apiteamsecuritypermissionsforgroup-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: The id of the group to find permissions for
      responses:
        200:
          description: OK
      tags:
      - This
      - Returns
      - Security
      - Permissions
      - That
      - Group
      - Has
      - "On"
      - Other
      - Groups
  /api/teamsecurity/permissionsongroup:
    get:
      summary: This returns security permissions that other groups have on specified
        group
      description: This returns security permissions that other groups have on specified
        group.
      operationId: TeamGroupSecurity_GetSecurityPermissionsThatApplyToGroupByteamId
      x-api-path-slug: apiteamsecuritypermissionsongroup-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: The id of the group to find other groups permissions
      responses:
        200:
          description: OK
      tags:
      - This
      - Returns
      - Security
      - Permissions
      - That
      - Other
      - Groups
      - Have
      - "On"
      - Specified
      - Group
  /api/todo/gettodosbyid:
    get:
      summary: Return list of tasks, corresponding to task ids passed in.
      description: Return list of tasks, corresponding to task ids passed in..
      operationId: DefaultToDo_GetTodosByIdByids
      x-api-path-slug: apitodogettodosbyid-get
      parameters:
      - in: query
        name: ids
        description: List of task ids
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Tasks
      - ""
      - Corresponding
      - To
      - Task
      - Ids
      - Passed
      - In
  /api/group/backgroundimages:
    get:
      summary: Return all background images.
      description: Return all background images..
      operationId: Group_BackgroundImagesBypageSizeBypageNumber
      x-api-path-slug: apigroupbackgroundimages-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Background
      - Images
  /api/group/updateprimarygroupmember:
    put:
      summary: Return the Groups with appointments between a given date range, ordered
        by appointments Count
      description: Return the groups with appointments between a given date range,
        ordered by appointments count.
      operationId: Group_UpdatePrimaryGroupMemberByfilter
      x-api-path-slug: apigroupupdateprimarygroupmember-put
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Appointments
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Appointments
      - Count
  /api/group/mostactive:
    get:
      summary: Return the Groups with the most viewings between a given date range,
        ordered by viewing Count
      description: Return the groups with the most viewings between a given date range,
        ordered by viewing count.
      operationId: Group_MostActiveBypageSizeByfilter.rangeFromByfilter.rangeToByfilter.branchIdByfilter.roleTypes
      x-api-path-slug: apigroupmostactive-get
      parameters:
      - in: query
        name: filter.branchId
      - in: query
        name: filter.rangeFrom
      - in: query
        name: filter.rangeTo
      - in: query
        name: filter.roleTypes
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Most
      - Viewings
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Viewing
      - Count
  /api/group/basicapplicantheatmap:
    get:
      summary: Return the lat and longs for every applicant in the system
      description: Return the lat and longs for every applicant in the system.
      operationId: Group_BasicApplicantHeatMapBypageSizeByfilter.rangeFromByfilter.rangeToByfilter.branchIdByfilter.rol
      x-api-path-slug: apigroupbasicapplicantheatmap-get
      parameters:
      - in: query
        name: filter.branchId
      - in: query
        name: filter.rangeFrom
      - in: query
        name: filter.rangeTo
      - in: query
        name: filter.roleTypes
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Lat
      - Longsevery
      - Applicant
      - In
      - System
  /api/group/{id}/properties:
    get:
      summary: Return a list of properties that the group owns
      description: Return a list of properties that the group owns.
      operationId: Group_GroupPropertiesByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidproperties-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Properties
      - That
      - Group
      - Owns
  /api/invoice/saveforlater:
    get:
      summary: Return list of receipts progress amounts
      description: Return list of receipts progress amounts.
      operationId: Invoice_SaveForLater
      x-api-path-slug: apiinvoicesaveforlater-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Receipts
      - Progress
      - Amounts
  /api/invoice/getreceiptitems:
    get:
      summary: Return list of receipts to process
      description: Return list of receipts to process.
      operationId: Invoice_GetSavedReceiptItemsForAgency
      x-api-path-slug: apiinvoicegetreceiptitems-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Receipts
      - To
      - Process
  /api/negotiator/my/properties/{roleType}:
    get:
      summary: Used for the Property Sales Dashboard to return a list of the negotiator's
        properties.
      description: Used for the property sales dashboard to return a list of the negotiator's
        properties..
      operationId: Negotiator_PropertiesByroleTypeBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesroletype-get
      parameters:
      - in: query
        name: pageNumber
        description: which page number of results to choose
      - in: query
        name: pageSize
        description: how many properties to return (default 10)
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleType
        description: the PropertyMarketingRole type
      responses:
        200:
          description: OK
      tags:
      - Usedthe
      - Property
      - Sales
      - Dashboard
      - To
      - Return
      - List
      - Of
      - Negotiators
      - Properties
  /api/negotiator/my/keys:
    get:
      summary: Return all Negotiator keys for the side bar display.
      description: Return all negotiator keys for the side bar display..
      operationId: Negotiator_KeysBypageSizeBypageNumberBycheckedOutOnly
      x-api-path-slug: apinegotiatormykeys-get
      parameters:
      - in: query
        name: checkedOutOnly
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Negotiator
      - Keysthe
      - Side
      - Bar
      - Display
  /api/negotiator/intervaleventcounts:
    post:
      summary: Return interval based event counts for negotiators.
      description: Return interval based event counts for negotiators..
      operationId: Negotiator_IntervalEventCountsByintervalEventCountDataContract
      x-api-path-slug: apinegotiatorintervaleventcounts-post
      parameters:
      - in: body
        name: intervalEventCountDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Interval
      - Based
      - Event
      - Countsnegotiators
  /api/property/comparables:
    get:
      summary: For a given property, will return all comparable property's nearby.
      description: For a given property, will return all comparable property's nearby..
      operationId: Property_ComparablesBypropertyIdBylatitudeBylongitudeBymileRadiusBypageSizeBypageNumberBybranchIdByi
      x-api-path-slug: apipropertycomparables-get
      parameters:
      - in: query
        name: branchId
        description: Optional Branch Id
      - in: query
        name: isForLetting
        description: Indicate if the request is for Sales or Lettings
      - in: query
        name: latitude
        description: The latitude to find comparables for
      - in: query
        name: longitude
        description: The longitude to find comparables for
      - in: query
        name: mileRadius
        description: how near to compare (default 1 mile)
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: query
        name: propertyId
        description: The id of the property to find comparables for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - For
      - Given
      - Property
      - ""
      - Will
      - Return
      - ""
      - Comparable
      - Propertys
      - Nearby
  /api/property/{id}/owners:
    get:
      summary: For a given property, will return owning PeopleGroup
      description: For a given property, will return owning peoplegroup.
      operationId: Property_OwnersByid
      x-api-path-slug: apipropertyidowners-get
      parameters:
      - in: path
        name: id
        description: property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - For
      - Given
      - Property
      - ""
      - Will
      - Return
      - Owning
      - PeopleGroup
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