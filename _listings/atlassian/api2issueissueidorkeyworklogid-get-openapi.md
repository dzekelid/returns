---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get worklog
  description: "Returns a specific worklog.  \n**Note:** The work log won't be returned
    if the Log work field is hidden for the project."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/application-properties:
    get:
      summary: Get application property
      description: Returns an application property.
      operationId: com.atlassian.jira.rest.v2.admin.ApplicationPropertiesResource.getApplicationProperty_get
      x-api-path-slug: api2applicationproperties-get
      parameters:
      - in: query
        name: key
        description: a String containing the property key
      - in: query
        name: keyFilter
        description: when fetching a list allows the list to be filtered by the propertys
          start of key e
      - in: query
        name: permissionLevel
        description: when fetching a list specifies the permission level of all items
          in the list see {@link com
      responses:
        200:
          description: OK
      tags:
      - Application
      - Property
  /api/2/application-properties/advanced-settings:
    get:
      summary: Get advanced settings
      description: Returns the properties that are displayed on the General Configuration
        Advanced Settings page.
      operationId: com.atlassian.jira.rest.v2.admin.ApplicationPropertiesResource.getAdvancedSettings_get
      x-api-path-slug: api2applicationpropertiesadvancedsettings-get
      responses:
        200:
          description: OK
      tags:
      - Advanced
      - Settings
  /api/2/applicationrole:
    get:
      summary: Get all application roles
      description: Returns all ApplicationRoles in the system. Will also return an
        ETag header containing a version hash of the collection of ApplicationRoles.
      operationId: com.atlassian.jira.rest.v2.admin.applicationrole.ApplicationRoleResource.getAllApplicationRoles_get
      x-api-path-slug: api2applicationrole-get
      responses:
        200:
          description: OK
      tags:
      - Application
      - Roles
  /api/2/applicationrole/{key}:
    get:
      summary: Get application role
      description: Returns the ApplicationRole with passed key if it exists.
      operationId: com.atlassian.jira.rest.v2.admin.applicationrole.ApplicationRoleResource.getApplicationRole_get
      x-api-path-slug: api2applicationrolekey-get
      parameters:
      - in: path
        name: key
        description: the key of the role to use
      responses:
        200:
          description: OK
      tags:
      - Application
      - Role
  /api/2/attachment/meta:
    get:
      summary: Get global attachment settings
      description: "Returns the global attachment settings, that is, whether attachments
        are enabled and the maximum attachment size allowed.  \n  \nNote that there
        are also [project permissions](https://confluence.atlassian.com/x/yodKLg)
        that restrict whether users can create and delete attachments or not.  \n
        \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
        None."
      operationId: com.atlassian.jira.rest.v2.issue.attachment.AttachmentResource.getAttachmentMeta_get
      x-api-path-slug: api2attachmentmeta-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Attachment
      - Settings
  /api/2/attachment/{id}:
    get:
      summary: Get attachment metadata
      description: "Returns the metadata for an attachment. Note that the attachment
        itself is not returned.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** None, however the calling user must have permission to view the
        issue that the attachment belongs to."
      operationId: com.atlassian.jira.rest.v2.issue.attachment.AttachmentResource.getAttachment_get
      x-api-path-slug: api2attachmentid-get
      parameters:
      - in: path
        name: id
        description: The ID of the attachment
      responses:
        200:
          description: OK
      tags:
      - Attachment
      - Metadata
  /api/2/attachment/{id}/expand/human:
    get:
      summary: Get all metadata for an expanded attachment
      description: "Returns the metadata for the contents of an attachment, if it
        is an archive, and metadata for the attachment itself. For example, if the
        attachment is a ZIP archive, then information about the files in the archive
        is returned and metadata for the ZIP archive. Currently, only the ZIP archive
        format is supported.  \n  \nUse this method to retrieve data that is presented
        in the UI, as this method returns the metadata for the attachment itself,
        such as the attachment's ID and name. Otherwise, use [Get contents metadata
        for an expanded attachment](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-attachment-id-expand-raw-get),
        which only returns the metadata for the attachment's contents.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** None, however the calling user must have permission to view the
        issue that the attachment belongs to."
      operationId: com.atlassian.jira.rest.v2.issue.attachment.AttachmentResource.expandAttachmentForHumans_get
      x-api-path-slug: api2attachmentidexpandhuman-get
      parameters:
      - in: path
        name: id
        description: The ID of the attachment
      responses:
        200:
          description: OK
      tags:
      - Metadataan
      - Expanded
      - Attachment
  /api/2/attachment/{id}/expand/raw:
    get:
      summary: Get contents metadata for an expanded attachment
      description: "Returns the metadata for the contents of an attachment, if it
        is an archive. For example, if the attachment is a ZIP archive, then information
        about the files in the archive is returned. Currently, only the ZIP archive
        format is supported.  \n  \nUse this method if you are processing the data
        without presenting it in the UI, as this method only returns the metadata
        for the contents of the attachment. Otherwise, to retrieve data to present
        in the UI, use [Get all metadata for an expanded attachment](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-attachment-id-expand-human-get)
        which also returns the metadata for the attachment itself, such as the attachment's
        ID and name.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** None, however the calling user must have permission to view the
        issue that the attachment belongs to."
      operationId: com.atlassian.jira.rest.v2.issue.attachment.AttachmentResource.expandAttachmentForMachines_get
      x-api-path-slug: api2attachmentidexpandraw-get
      parameters:
      - in: path
        name: id
        description: The ID of the attachment
      responses:
        200:
          description: OK
      tags:
      - Contents
      - Metadataan
      - Expanded
      - Attachment
  /api/2/auditing/record:
    get:
      summary: Get audit records
      description: Returns auditing records filtered using provided parameters
      operationId: com.atlassian.jira.rest.v2.admin.auditing.AuditingResource.getAuditRecords_get
      x-api-path-slug: api2auditingrecord-get
      parameters:
      - in: query
        name: filter
        description: \- text query; each record that will be returned must contain
          the provided text in one of its fields
      - in: query
        name: from
        description: \- timestamp in past; from must be less or equal to, otherwise
          the result set will be empty only records that where created in the same
          moment or after the from timestamp will be provided in response
      - in: query
        name: limit
        description: '\- maximum number of returned results (if is limit is  1000,
          it will be set do default value: 1000)'
      - in: query
        name: offset
        description: \- the number of record from which search starts
      - in: query
        name: to
        description: \- timestamp in past; from must be less or equal to, otherwise
          the result set will be empty only records that where created in the same
          moment or earlier than the to timestamp will be provided in response
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Records
  /api/2/avatar/{type}/system:
    get:
      summary: Get all system avatars
      description: Returns all system avatars of the given type.
      operationId: com.atlassian.jira.rest.v2.issue.AvatarResource.getAllSystemAvatars_get
      x-api-path-slug: api2avatartypesystem-get
      parameters:
      - in: path
        name: type
        description: the avatar type
      responses:
        200:
          description: OK
      tags:
      - System
      - Avatars
  /api/2/comment/list:
    post:
      summary: Get comments by ids
      description: Returns comments for given comments ids. Only comments to which
        the user has permissions, will be included in the result. The returned set
        of comments is limited to 1000 elements.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentListResource.getCommentsByIds_post
      x-api-path-slug: api2commentlist-post
      parameters:
      - in: query
        name: expand
        description: 'optional comma separated list of parameters to expand: renderedBody
          (provides body rendered in HTML), properties (provides comment properties)'
      responses:
        200:
          description: OK
      tags:
      - Comments
      - By
      - Ids
  /api/2/comment/{commentId}/properties:
    get:
      summary: Get comment property keys
      description: Returns the keys of all properties for the comment identified by
        the key or by the id.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.getCommentPropertyKeys_get
      x-api-path-slug: api2commentcommentidproperties-get
      parameters:
      - in: path
        name: commentId
        description: the comment from which keys will be returned
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
      - Keys
  /api/2/comment/{commentId}/properties/{propertyKey}:
    get:
      summary: Get comment property
      description: Returns the value of the property with a given key from the comment
        identified by the key or by the id. The user who retrieves the property is
        required to have permissions to read the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.getCommentProperty_get
      x-api-path-slug: api2commentcommentidpropertiespropertykey-get
      parameters:
      - in: path
        name: commentId
        description: the comment from which the property will be returned
      - in: path
        name: propertyKey
        description: the key of the property to return
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
  /api/2/component/{id}:
    get:
      summary: Get component
      description: 'Returns a component. [Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required: _Browse projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).'
      operationId: com.atlassian.jira.rest.v2.issue.ComponentResource.getComponent_get
      x-api-path-slug: api2componentid-get
      parameters:
      - in: path
        name: id
        description: The ID of the component
      responses:
        200:
          description: OK
      tags:
      - Component
  /api/2/component/{id}/relatedIssueCounts:
    get:
      summary: Get component issues count
      description: Returns the counts of issues assigned to the component. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira.
      operationId: com.atlassian.jira.rest.v2.issue.ComponentResource.getComponentRelatedIssues_get
      x-api-path-slug: api2componentidrelatedissuecounts-get
      parameters:
      - in: path
        name: id
        description: The ID of the component
      responses:
        200:
          description: OK
      tags:
      - Component
      - Issues
      - Count
  /api/2/configuration:
    get:
      summary: Get global settings
      description: "Returns the [global settings](https://confluence.atlassian.com/x/qYXKM)
        in Jira. These settings determine whether optional features (for example,
        sub-tasks, time tracking, and others) are enabled. If time tracking is enabled,
        this method also returns the time tracking configuration.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.ConfigurationResource.getConfiguration_get
      x-api-path-slug: api2configuration-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Settings
  /api/2/configuration/timetracking:
    get:
      summary: Get selected time tracking provider
      description: "Returns the time tracking provider that is currently selected.
        Note that if time tracking is disabled, then a successful but empty response
        is returned.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.getSelectedTimeTrackingImplementa
      x-api-path-slug: api2configurationtimetracking-get
      responses:
        200:
          description: OK
      tags:
      - Selected
      - Time
      - Tracking
      - Provider
  /api/2/configuration/timetracking/list:
    get:
      summary: Get all time tracking providers
      description: "Returns all time tracking providers. By default, Jira only has
        one time tracking provider: _JIRA provided time tracking_. However, you can
        install other time tracking providers via apps from the Atlassian Marketplace.
        For more information on time tracking providers, see the documentation for
        the [Time Tracking Provider](https://developer.atlassian.com/cloud/jira/platform/modules/time-tracking-provider/)
        module.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.getAvailableTimeTrackingImplement
      x-api-path-slug: api2configurationtimetrackinglist-get
      responses:
        200:
          description: OK
      tags:
      - Time
      - Tracking
      - Providers
  /api/2/configuration/timetracking/options:
    get:
      summary: Get time tracking settings
      description: "Returns the time tracking settings. This includes settings such
        as the time format, default time unit, and others. For more information, see
        [Configuring time tracking](https://confluence.atlassian.com/x/qoXKM).  \n
        \ \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.getSharedTimeTrackingConfiguratio
      x-api-path-slug: api2configurationtimetrackingoptions-get
      responses:
        200:
          description: OK
      tags:
      - Time
      - Tracking
      - Settings
  /api/2/customFieldOption/{id}:
    get:
      summary: Get custom field option
      description: "Returns a custom field option. For example, an option in a cascading
        select list.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** None."
      operationId: com.atlassian.jira.rest.v2.issue.customfield.CustomFieldOptionResource.getCustomFieldOption_get
      x-api-path-slug: api2customfieldoptionid-get
      parameters:
      - in: path
        name: id
        description: The ID of the custom field option
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Field
      - Option
  /api/2/dashboard:
    get:
      summary: Get all dashboards
      description: "Returns a list of dashboards owned by or shared with the user.
        The list may be filtered to include only favorite or owned dashboards.  \n
        \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
        Permission to access Jira."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardResource.getAllDashboards_get
      x-api-path-slug: api2dashboard-get
      parameters:
      - in: query
        name: filter
        description: The filter applied to the list of dashboards
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      responses:
        200:
          description: OK
      tags:
      - Dashboards
  /api/2/dashboard/{dashboardId}/items/{itemId}/properties:
    get:
      summary: Get dashboard item property keys
      description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira. However, to get the property keys the
        user must be the owner of the dashboard or be shared the dashboard. Note,
        users with the _Administer Jira_ [global permission](href=) are considered
        owners of the System dashboard. The System dashboard is considered to be shared
        with all other users."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.getDashboardItemPropertyKeys_get
      x-api-path-slug: api2dashboarddashboardiditemsitemidproperties-get
      parameters:
      - in: path
        name: dashboardId
        description: The ID of the dashboard
      - in: path
        name: itemId
        description: The ID of the dashboard item
      responses:
        200:
          description: OK
      tags:
      - Dashboard
      - Item
      - Property
      - Keys
  /api/2/dashboard/{dashboardId}/items/{itemId}/properties/{propertyKey}:
    get:
      summary: Get dashboard item property
      description: "Returns the key and value of a dashboard item property.  \n  \nA
        dashboard item enables an app to add user-specific information to a user dashboard.
        Dashboard items are exposed to users as gadgets that users can add to their
        dashboards. For more information on how users do this, see [Adding and customizing
        gadgets](https://confluence.atlassian.com/x/7AeiLQ).  \n  \nWhen an app creates
        a dashboard item it registers a callback to receive the dashboard item ID.
        The callback fires whenever the item is rendered or, where the item is configurable,
        the user edits the item. The app then uses this resource to store the item's
        content or configuration details. For more information on working with dashboard
        items, see [Building a dashboard item for a JIRA Connect add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
        and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
        documentation.  \n  \nThere is no resource to set or get dashboard items.
        \ \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
        Permission to access Jira. However, to get a dashboard item property the user
        must be the owner of the dashboard or be shared the dashboard. Note, users
        with the _Administer Jira_ [global permission](href=) are considered owners
        of the System dashboard. The System dashboard is considered to be shared with
        all other users."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.getDashboardItemProperty_get
      x-api-path-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
      parameters:
      - in: path
        name: dashboardId
        description: The ID of the dashboard
      - in: path
        name: itemId
        description: The ID of the dashboard item
      - in: path
        name: propertyKey
        description: The key of the dashboard item property
      responses:
        200:
          description: OK
      tags:
      - Dashboard
      - Item
      - Property
  /api/2/dashboard/{id}:
    get:
      summary: Get dashboard
      description: "Returns a dashboard.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira. However, to get a dashboard, the dashboard
        must be shared with the user or the user must own it. Note, users with the
        _Administer Jira_ [global permission](href=) are considered owners of the
        System dashboard. The System dashboard is considered to be shared with all
        other users."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardResource.getDashboard_get
      x-api-path-slug: api2dashboardid-get
      parameters:
      - in: path
        name: id
        description: The ID of the dashboard
      responses:
        200:
          description: OK
      tags:
      - Dashboard
  /api/2/field:
    get:
      summary: Get fields
      description: |-
        Returns all issue fields in Jira, both system and custom fields.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however the following rules apply:

        *   Fields that cannot be added to the issue navigator are always returned.
        *   Fields that cannot be placed on an issue screen are always returned.
        *   Fields that depend on global Jira settings are only returned if the setting is enabled. That is, timetracking fields, subtasks, votes, and watches.
        *   For all other fields, this method only returns the fields that the current user has permission to see (that is, the field can be used in at least one project that the user can see).
      operationId: com.atlassian.jira.rest.v2.issue.FieldResource.getFields_get
      x-api-path-slug: api2field-get
      responses:
        200:
          description: OK
      tags:
      - Fields
  /api/2/field/{fieldKey}/option:
    get:
      summary: Get all issue field options
      description: |-
        Returns all options defined for a select list issue field. A select list issue field is a type of [issue field](https://developer.atlassian.com/cloud/jira/platform/modules/issue-field/) that allows a user to select an value from a list of options.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getAllIssueFieldOptions_get
      x-api-path-slug: api2fieldfieldkeyoption-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: startAt
        description: The starting index of the returned objects
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Options
  /api/2/field/{fieldKey}/option/suggestions/edit:
    get:
      summary: Get selectable issue field options
      description: |-
        Returns options defined for a select list issue field that can be viewed and selected by the currently logged in user.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to access Jira.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getSelectableIssueFieldOptions_get
      x-api-path-slug: api2fieldfieldkeyoptionsuggestionsedit-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: projectId
        description: Filters the results to options that are only available in the
          specified project
      - in: query
        name: startAt
        description: The starting index of the returned objects
      responses:
        200:
          description: OK
      tags:
      - Selectable
      - Issue
      - Field
      - Options
  /api/2/field/{fieldKey}/option/suggestions/search:
    get:
      summary: Get visible issue field options
      description: |-
        Returns options defined for a select list issue field that can be viewed by the currently logged in user.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to access Jira.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getVisibleIssueFieldOptions_get
      x-api-path-slug: api2fieldfieldkeyoptionsuggestionssearch-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: projectId
        description: Filters the results to options that are only available in the
          specified project
      - in: query
        name: startAt
        description: The starting index of the returned objects
      responses:
        200:
          description: OK
      tags:
      - Visible
      - Issue
      - Field
      - Options
  /api/2/field/{fieldKey}/option/{optionId}:
    get:
      summary: Get issue field option
      description: |-
        Returns an option from a select list issue field.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getIssueFieldOption_get
      x-api-path-slug: api2fieldfieldkeyoptionoptionid-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: path
        name: optionId
        description: The ID of the option to be returned
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
  /api/2/filter:
    get:
      summary: Get filters
      description: |-
        Returns all filters. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however only the following filters are returned:

        *   Filters owned by the user.
        *   Filters shared with a group that the user is a member of.
        *   Filters shared with a private project that the user can browse.
        *   Filters shared with a public project, even if the user is anonymous.
        *   Filters shared with the public, even if the user is anonymous.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getFilters_get
      x-api-path-slug: api2filter-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      responses:
        200:
          description: OK
      tags:
      - Filters
  /api/2/filter/defaultShareScope:
    get:
      summary: Get default share scope
      description: Returns the default sharing settings for new filters and dashboards
        for a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
        Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getDefaultShareScope_get
      x-api-path-slug: api2filterdefaultsharescope-get
      responses:
        200:
          description: OK
      tags:
      - Default
      - Share
      - Scope
  /api/2/filter/favourite:
    get:
      summary: Get favourite filters
      description: Returns the favorite filters of the calling user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getFavouriteFilters_get
      x-api-path-slug: api2filterfavourite-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      responses:
        200:
          description: OK
      tags:
      - Favourite
      - Filters
  /api/2/filter/my:
    get:
      summary: Get my filters
      description: Returns the filters owned by the calling user. If `includeFavourites`
        is `true`, the user's favorite filters are also returned. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getMyFilters_get
      x-api-path-slug: api2filtermy-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: query
        name: includeFavourites
        description: Include the users favorite filters in the response
      responses:
        200:
          description: OK
      tags:
      - My
      - Filters
  /api/2/filter/{id}:
    get:
      summary: Get filter
      description: Returns a filter. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** None, however the calling user must have permission view the filter.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getFilter_get
      x-api-path-slug: api2filterid-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: path
        name: id
        description: The ID of the filter to return
      responses:
        200:
          description: OK
      tags:
      - Filter
  /api/2/filter/{id}/columns:
    get:
      summary: Get columns
      description: Returns the columns configured for a filter. The column configuration
        is used when the filter's results are viewed in _List View_ with the _Columns_
        set to _Filter_. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** None, however the calling user must have permission to view the
        filter.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getColumns_get
      x-api-path-slug: api2filteridcolumns-get
      parameters:
      - in: path
        name: id
        description: The ID of the filter
      responses:
        200:
          description: OK
      tags:
      - Columns
  /api/2/filter/{id}/permission:
    get:
      summary: Get share permissions
      description: Returns the share permissions for a filter. A filter can be shared
        with groups, projects, all logged-in users, or the public. Sharing with all
        logged-in users or the public is known as a global share permission. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** None, however the calling user must have permission to view the
        filter.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getSharePermissions_get
      x-api-path-slug: api2filteridpermission-get
      parameters:
      - in: path
        name: id
        description: The ID of the filter
      responses:
        200:
          description: OK
      tags:
      - Share
      - Permissions
  /api/2/filter/{id}/permission/{permissionId}:
    get:
      summary: Get share permission
      description: Returns a share permission for a filter. A filter can be shared
        with groups, projects, all logged-in users, or the public. Sharing with all
        logged-in users or the public is known as a global share permission. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** None, however the calling user must have permission to view the
        filter.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.getSharePermission_get
      x-api-path-slug: api2filteridpermissionpermissionid-get
      parameters:
      - in: path
        name: id
        description: The ID of the filter
      - in: path
        name: permissionId
        description: The ID of the share permission
      responses:
        200:
          description: OK
      tags:
      - Share
      - Permission
  /api/2/group:
    get:
      summary: Get group
      description: |-
        This resource is deprecated, use [`group/member`](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-group-member-get).

        Returns all users in a group.

        **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
      operationId: com.atlassian.jira.rest.v2.issue.GroupResource.getGroup_get
      x-api-path-slug: api2group-get
      parameters:
      - in: query
        name: expand
        description: List of fields to expand
      - in: query
        name: groupname
        description: The name of the group
      responses:
        200:
          description: OK
      tags:
      - Group
  /api/2/group/member:
    get:
      summary: Get users from group
      description: |-
        Returns all users in a group. Users are ordered by username.

        **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
      operationId: com.atlassian.jira.rest.v2.issue.GroupResource.getUsersFromGroup_get
      x-api-path-slug: api2groupmember-get
      parameters:
      - in: query
        name: groupname
        description: The name of the group
      - in: query
        name: includeInactiveUsers
        description: Include inactive users
      - in: query
        name: maxResults
        description: The maximum number of users to return per page
      - in: query
        name: startAt
        description: The index of the first user to return
      responses:
        200:
          description: OK
      tags:
      - Users
      - From
      - Group
  /api/2/groups/picker:
    get:
      summary: Find groups
      description: |-
        Returns groups with substrings matching a given query. This is mainly for use with the group picker, so the returned groups contain html to be used as picker suggestions. The groups are also wrapped in a single response object that also contains a header for use in the picker, specifically _Showing X of Y matching groups_.

        The number of groups returned is limited by the system property "jira.ajax.autocomplete.limit"

        The groups will be unique and sorted.
      operationId: com.atlassian.jira.rest.v2.issue.GroupPickerResource.findGroups_get
      x-api-path-slug: api2groupspicker-get
      parameters:
      - in: query
        name: accountId
      - in: query
        name: exclude
      - in: header
        name: force-account-id
      - in: query
        name: maxResults
      - in: query
        name: query
        description: a String to match groups agains
      - in: query
        name: userName
      responses:
        200:
          description: OK
      tags:
      - Find
      - Groups
  /api/2/groupuserpicker:
    get:
      summary: Find users and groups
      description: Returns a list of users and groups matching query with highlighting.
        This resource cannot be accessed anonymously.
      operationId: com.atlassian.jira.rest.v2.issue.GroupAndUserPickerResource.findUsersAndGroups_get
      x-api-path-slug: api2groupuserpicker-get
      parameters:
      - in: query
        name: avatarSize
        description: The size of the avatar to return
      - in: query
        name: caseInsensitive
        description: whether the search for groups should be case insensitive
      - in: query
        name: excludeConnectAddons
        description: Boolean indicating whether Connect Add-on users and groups should
          be excluded from the search results
      - in: query
        name: fieldId
        description: The custom field id, if this request comes from a custom field,
          such as a user picker
      - in: query
        name: issueTypeId
        description: The list of issue type ids to further restrict the search
      - in: query
        name: maxResults
        description: the maximum number of users to return (defaults to 50)
      - in: query
        name: projectId
        description: The list of project ids to further restrict the search This parameter
          can occur multiple times to pass in multiple project ids
      - in: query
        name: query
        description: A string used to search username, Name or e-mail address
      - in: query
        name: showAvatar
        description: If the user avatar should be returned or not
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - Groups
  /api/2/issue/createmeta:
    get:
      summary: Get create issue meta
      description: |-
        Returns the metadata for creating issues. This includes the available projects, issue types, fields (with information whether those fields are required) and field types. Projects, in which the user does not have permission to create issues, will not be returned.

        The fields in the createmeta response correspond to the fields on the issue's Create screen for the specific project/issuetype. Fields hidden from the screen will not be returned in the createmeta response.

        Fields will only be returned if `expand=projects.issuetypes.fields` is set.

        The results can be filtered by project and/or issue type, controlled by the query parameters.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getCreateIssueMeta_get
      x-api-path-slug: api2issuecreatemeta-get
      parameters:
      - in: query
        name: issuetypeIds
        description: Multi-value parameter defining issue type IDs to be used for
          the results filtering
      - in: query
        name: issuetypeNames
        description: Multi-value parameter defining issue type names to be used for
          the results filtering
      - in: query
        name: projectIds
        description: Multi-value parameter defining project IDs to be used for the
          results filtering
      - in: query
        name: projectKeys
        description: Multi-value parameter defining project keys to be used for the
          results filtering
      responses:
        200:
          description: OK
      tags:
      - Create
      - Issue
      - Meta
  /api/2/issue/picker:
    get:
      summary: Get issue picker resource
      description: Returns a list of suggested issues matching the auto-completion
        query for the user executing this request. This REST method checks the user's
        history and browsing context to return issue suggestions.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getIssuePickerResource_get
      x-api-path-slug: api2issuepicker-get
      parameters:
      - in: query
        name: currentIssueKey
        description: Key of the issue defining search context
      - in: query
        name: currentJQL
        description: JQL defining search context
      - in: query
        name: currentProjectId
        description: ID of a project defining search context
      - in: query
        name: query
        description: Query used to filter issue search results
      - in: query
        name: showSubTaskParent
        description: Set to false to exclude parent issue from the suggestions list
          if search is performed in the context of a sub-task
      - in: query
        name: showSubTasks
        description: Set to false to exclude subtasks from the suggestions list
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Picker
      - Resource
  /api/2/issue/{issueIdOrKey}:
    get:
      summary: Get issue
      description: |-
        Returns a full representation of the issue for the given issue key.

        The issue JSON consists of the issue key and a collection of fields. Additional information like links to workflow transition sub-resources, or HTML rendered values of the fields supporting HTML rendering can be retrieved with `expand` request parameter specified.

        The `fields` request parameter accepts a comma-separated list of fields to include in the response. It can be used to retrieve a subset of fields. By default all fields are returned in the response. A particular field can be excluded from the response if prefixed with a "-" (minus) sign. Parameter can be provided multiple times on a single request.

        By default, all fields are returned in the response. Note: this is different from a JQL search - only navigable fields are returned by default (`*navigable`).
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getIssue_get
      x-api-path-slug: api2issueissueidorkey-get
      parameters:
      - in: query
        name: expand
        description: Multi-value parameter defining the additional issue attributes
          to be included in the response
      - in: query
        name: fields
        description: Multi-value parameter defining the fields returned for the issue
      - in: query
        name: fieldsByKeys
        description: If true then issue fields are referenced by keys instead of IDs
      - in: path
        name: issueIdOrKey
        description: 'ID or key of the issue, for example: JRACLOUD-1549'
      - in: query
        name: properties
        description: Multi-value parameter defining the list of properties returned
          for the issue
      - in: query
        name: updateHistory
        description: If set to true, adds the issue retrieved by this method to the
          current users issue history
      responses:
        200:
          description: OK
      tags:
      - Issue
  /api/2/issue/{issueIdOrKey}/changelog:
    get:
      summary: Get change logs
      description: Returns a [paginated](#pagination) list of all updates of an issue,
        sorted by date, starting from the oldest.
      operationId: com.atlassian.jira.rest.v2.issue.IssueChangelogResource.getChangeLogs_get
      x-api-path-slug: api2issueissueidorkeychangelog-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue
      - in: query
        name: maxResults
        description: Maximum number of items to return per page
      - in: query
        name: startAt
        description: Page offset, ie
      responses:
        200:
          description: OK
      tags:
      - Change
      - Logs
  /api/2/issue/{issueIdOrKey}/comment:
    get:
      summary: Get comments
      description: |-
        Returns all comments for an issue.

        Results can be ordered by the "created" field which means the date a comment was added.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentResource.getComments_get
      x-api-path-slug: api2issueissueidorkeycomment-get
      parameters:
      - in: query
        name: expand
        description: 'optional flags: renderedBody (provides body rendered in HTML)'
      - in: path
        name: issueIdOrKey
        description: to get comments for
      - in: query
        name: maxResults
        description: how many results on the page should be included
      - in: query
        name: orderBy
        description: ordering of the results
      - in: query
        name: startAt
        description: the page offset, if not specified then defaults to 0
      responses:
        200:
          description: OK
      tags:
      - Comments
  /api/2/issue/{issueIdOrKey}/comment/{id}:
    get:
      summary: Get comment
      description: Returns a single comment.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentResource.getComment_get
      x-api-path-slug: api2issueissueidorkeycommentid-get
      parameters:
      - in: query
        name: expand
        description: 'optional flags: renderedBody (provides body rendered in HTML)'
      - in: path
        name: id
        description: the ID of the comment to request
      - in: path
        name: issueIdOrKey
        description: of the issue the comment belongs to
      responses:
        200:
          description: OK
      tags:
      - Comment
  /api/2/issue/{issueIdOrKey}/editmeta:
    get:
      summary: Get edit issue meta
      description: |-
        Returns the metadata for editing an issue.

        The fields returned by editmeta resource are the ones shown on the issue's Edit screen. Fields hidden from the screen will not be returned unless `overrideScreenSecurity` parameter is set to true.

        If an issue cannot be edited in Jira because of its workflow status (for example the issue is closed), then no fields will be returned, unless `overrideEditableFlag` is set to true.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getEditIssueMeta_get
      x-api-path-slug: api2issueissueidorkeyeditmeta-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue
      - in: query
        name: overrideEditableFlag
        description: Allows retrieving edit metadata for fields in non-editable status
          (jira
      - in: query
        name: overrideScreenSecurity
        description: Allows retrieving edit metadata for the fields hidden on Edit
          screen
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Issue
      - Meta
  /api/2/issue/{issueIdOrKey}/properties:
    get:
      summary: Get issue property keys
      description: Returns the keys of all properties for the issue identified by
        the key or by the id.
      operationId: com.atlassian.jira.rest.v2.issue.IssuePropertyResource.getIssuePropertyKeys_get
      x-api-path-slug: api2issueissueidorkeyproperties-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue from which keys will be returned
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Property
      - Keys
  /api/2/issue/{issueIdOrKey}/properties/{propertyKey}:
    get:
      summary: Get issue property
      description: Returns the value of the property with a given key from the issue
        identified by the key or by the id. The user who retrieves the property is
        required to have permissions to read the issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssuePropertyResource.getIssueProperty_get
      x-api-path-slug: api2issueissueidorkeypropertiespropertykey-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue from which the property will be returned
      - in: path
        name: propertyKey
        description: the key of the property to return
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Property
  /api/2/issue/{issueIdOrKey}/remotelink:
    get:
      summary: Get remote issue links
      description: Returns the remote issue links for the issue. This may be links
        to other Jira instances, web applications or web pages.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getRemoteIssueLinks_get
      x-api-path-slug: api2issueissueidorkeyremotelink-get
      parameters:
      - in: query
        name: globalId
        description: ID of the remote issue link to be returned
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve remote links for
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Links
  /api/2/issue/{issueIdOrKey}/remotelink/{linkId}:
    get:
      summary: Get remote issue link by id
      description: Returns the remote issue link by the given ID.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getRemoteIssueLinkById_get
      x-api-path-slug: api2issueissueidorkeyremotelinklinkid-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve the remote issue links for
      - in: path
        name: linkId
        description: ID of the remote issue link
      responses:
        200:
          description: OK
      tags:
      - Remote
      - Issue
      - Link
      - By
      - Id
  /api/2/issue/{issueIdOrKey}/transitions:
    get:
      summary: Get transitions
      description: |-
        Returns a list of transitions available for this issue for the current user.

        Specify `expand=transitions.fields` parameter to retrieve the fields required for a transition together with their types.

        Fields metadata corresponds to the fields available in a transition screen for a particular transition. Fields hidden from the screen will not be returned in the metadata.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getTransitions_get
      x-api-path-slug: api2issueissueidorkeytransitions-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to return transitions for
      - in: query
        name: skipRemoteOnlyCondition
        description: Flag to skip evaluation of {@link RemoteOnlyCondition}
      - in: query
        name: transitionId
      responses:
        200:
          description: OK
      tags:
      - Transitions
  /api/2/issue/{issueIdOrKey}/votes:
    get:
      summary: Get votes
      description: Returns voting data for an issue - whether the issue was voted
        for, total number of votes and users who voted for the issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getVotes_get
      x-api-path-slug: api2issueissueidorkeyvotes-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve voting information for
      responses:
        200:
          description: OK
      tags:
      - Votes
  /api/2/issue/{issueIdOrKey}/watchers:
    get:
      summary: Get issue watchers
      description: Returns the list of watchers for the issue with the given key.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getIssueWatchers_get
      x-api-path-slug: api2issueissueidorkeywatchers-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve watchers for
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Watchers
  /api/2/issue/{issueIdOrKey}/worklog:
    get:
      summary: Get issue worklog
      description: "Returns all work logs for an issue. The response is [paginated](#pagination)
        \ \n**Note:** Work logs won't be returned if the Log work field is hidden
        for the project."
      operationId: com.atlassian.jira.rest.v2.issue.IssueWorklogsResource.getIssueWorklog_get
      x-api-path-slug: api2issueissueidorkeyworklog-get
      parameters:
      - in: query
        name: expand
        description: 'Optional comma separated list of parameters to expand: properties
          (provides worklog properties)'
      - in: path
        name: issueIdOrKey
        description: The worklogs belongs to
      - in: query
        name: maxResults
        description: Maximum number of items to return per page
      - in: query
        name: startAt
        description: Page offset, ie
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Worklog
  /api/2/issue/{issueIdOrKey}/worklog/{id}:
    get:
      summary: Get worklog
      description: "Returns a specific worklog.  \n**Note:** The work log won't be
        returned if the Log work field is hidden for the project."
      operationId: com.atlassian.jira.rest.v2.issue.IssueWorklogsResource.getWorklog_get
      x-api-path-slug: api2issueissueidorkeyworklogid-get
      parameters:
      - in: query
        name: expand
        description: 'optional comma separated list of parameters to expand: properties
          (provides worklog properties)'
      - in: path
        name: id
        description: a String containing the work log id
      - in: path
        name: issueIdOrKey
        description: a string containing the issue id or key the worklog belongs to
      responses:
        200:
          description: OK
      tags:
      - Worklog
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