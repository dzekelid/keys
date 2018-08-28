---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get change logs
  description: Returns a [paginated](#pagination) list of all updates of an issue,
    sorted by date, starting from the oldest.
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
  /api/2/issue/{issueIdOrKey}/worklog/{worklogId}/properties:
    get:
      summary: Get worklog property keys
      description: Returns the keys of all properties for the worklog identified by
        the key or by the id.
      operationId: com.atlassian.jira.rest.v2.issue.WorklogPropertyResource.getWorklogPropertyKeys_get
      x-api-path-slug: api2issueissueidorkeyworklogworklogidproperties-get
      parameters:
      - in: path
        name: issueIdOrKey
      - in: path
        name: worklogId
        description: the worklog from which keys will be returned
      responses:
        200:
          description: OK
      tags:
      - Worklog
      - Property
      - Keys
  /api/2/issuetype/{issueTypeId}/properties:
    get:
      summary: Get issue type property keys
      description: |-
        Returns all the [issue type property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys of the issue type. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   _Administer Jira_ [global permission](href=) to get the property keys of any issue type.
        *   _Browse projects_ project permission to get the property keys of any issue types associated with the projects the user has permission to browse.
      operationId: com.atlassian.jira.rest.v2.issue.IssueTypePropertyResource.getIssueTypePropertyKeys_get
      x-api-path-slug: api2issuetypeissuetypeidproperties-get
      parameters:
      - in: path
        name: issueTypeId
        description: The ID of the issue type
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Type
      - Property
      - Keys
  /api/2/project/{projectIdOrKey}/properties:
    get:
      summary: Get project property keys
      description: |-
        Returns all [project property](https://developer.atlassian.com/cloud/jira/platform/storing-data-without-a-database/#a-id-jira-entity-properties-a-jira-entity-properties) keys for the project.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.ProjectPropertyResource.getProjectPropertyKeys_get
      x-api-path-slug: api2projectprojectidorkeyproperties-get
      parameters:
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      responses:
        200:
          description: OK
      tags:
      - Project
      - Property
      - Keys
  /api/2/user/properties:
    get:
      summary: Get user property keys
      description: |-
        Returns all property keys on a user. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To access the property keys on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To access the calling user's property keys: None

        Note: These user properties are unrelated to the [Jira properties](https://confluence.atlassian.com/cloud/add-data-to-users-for-advanced-functions-jira-applications-only-744721649.html) that can be set through the UI.
      operationId: com.atlassian.jira.rest.v2.userproperty.UserPropertyResource.getUserPropertyKeys_get
      x-api-path-slug: api2userproperties-get
      parameters:
      - in: query
        name: accountId
        description: The account ID of the user
      - in: header
        name: force-account-id
      - in: query
        name: userKey
        description: The key of the user
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - User
      - Property
      - Keys
  /api/2/user/search/query/key:
    get:
      summary: Find user keys by query
      description: |-
        Finds users using a structured query and returns a list of user keys. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse users and groups_ [global permission](href=). The available query statements are:

        *   `is assignee of PROJ` Returns the users that are assignees of at least one issue in project _PROJ_.
        *   `is assignee of (PROJ-1, PROJ-2)` Returns users that are assignees on the issues _PROJ-1_ or _PROJ-2_.
        *   `is reporter of (PROJ-1, PROJ-2)` Returns users that are reporters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is watcher of (PROJ-1, PROJ-2)` Returns users that are watchers on the issues _PROJ-1_ or _PROJ-2_.
        *   `is voter of (PROJ-1, PROJ-2)` Returns users that are voters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is commenter of (PROJ-1, PROJ-2)` Returns users that have posted a comment on the issues _PROJ-1_ or _PROJ-2_.
        *   `is transitioner of (PROJ-1, PROJ-2)` Returns users that have performed a transition on issues _PROJ-1_ or _PROJ-2_.
        *   `[propertyKey].entity.property.path is "property value"` Returns users with the entity property value.

        The list of issues can be extended as needed, as in _(PROJ-1, PROJ-2, ... PROJ-n)_. Statements can be combined using the `AND` and `OR` operators to form more complex queries, for example:

        `is assignee of PROJ AND [propertyKey].entity.property.path is "property value"`
      operationId: com.atlassian.jira.rest.v2.search.UserSearchResource.findUserKeysByQuery_get
      x-api-path-slug: api2usersearchquerykey-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: includeInactive
        description: Include inactive users in the results
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: query
        description: The search query
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      responses:
        200:
          description: OK
      tags:
      - Find
      - User
      - Keys
      - By
      - Query
  /api/2/project/type/{projectTypeKey}:
    get:
      summary: Get project type by key
      description: |-
        Returns a [project type](https://confluence.atlassian.com/x/Var1Nw).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira (that is, member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.project.type.ProjectTypeResource.getProjectTypeByKey_get
      x-api-path-slug: api2projecttypeprojecttypekey-get
      parameters:
      - in: path
        name: projectTypeKey
        description: The key of the project type
      responses:
        200:
          description: OK
      tags:
      - Project
      - Type
      - By
      - Key
  /api/2/project/type/{projectTypeKey}/accessible:
    get:
      summary: Get accessible project type by key
      description: |-
        Returns a [project type](https://confluence.atlassian.com/x/Var1Nw) if it is accessible to the logged in user.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira (that is, member of the _users_ [group](https://confluence.atlassian.com/x/24xjL)).
      operationId: com.atlassian.jira.rest.v2.project.type.ProjectTypeResource.getAccessibleProjectTypeByKey_get
      x-api-path-slug: api2projecttypeprojecttypekeyaccessible-get
      parameters:
      - in: path
        name: projectTypeKey
        description: The key of the project type
      responses:
        200:
          description: OK
      tags:
      - Accessible
      - Project
      - Type
      - By
      - Key
  /api/2/projectvalidate/key:
    get:
      summary: Validate project key
      description: Validates a project key.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectValidateResource.validateProjectKey_get
      x-api-path-slug: api2projectvalidatekey-get
      parameters:
      - in: query
        name: key
        description: the project key
      responses:
        200:
          description: OK
      tags:
      - Validate
      - Project
      - Key
  /api/2/projectvalidate/validProjectKey:
    get:
      summary: Get valid project key
      description: Validates the project key and generated a valid project key if
        the supplied key is invalid.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectValidateResource.getValidProjectKey_get
      x-api-path-slug: api2projectvalidatevalidprojectkey-get
      parameters:
      - in: query
        name: key
        description: the project key
      responses:
        200:
          description: OK
      tags:
      - Valid
      - Project
      - Key
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
    put:
      summary: Set comment property
      description: |-
        Sets the value of the specified comment's property.

        You can use this resource to store a custom data against the comment identified by the key or by the id. The user who stores the data is required to have permissions to administer the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.setCommentProperty_put
      x-api-path-slug: api2commentcommentidpropertiespropertykey-put
      parameters:
      - in: path
        name: commentId
        description: the comment on which the property will be set
      - in: path
        name: propertyKey
        description: the key of the comments property
      responses:
        200:
          description: OK
      tags:
      - Set
      - Comment
      - Property
    delete:
      summary: Delete comment property
      description: Removes the property from the comment identified by the key or
        by the id. Ths user removing the property is required to have permissions
        to administer the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.deleteCommentProperty_delete
      x-api-path-slug: api2commentcommentidpropertiespropertykey-delete
      parameters:
      - in: path
        name: commentId
        description: the comment from which the property will be removed
      - in: path
        name: propertyKey
        description: the key of the property to remove
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
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
    put:
      summary: Set dashboard item property
      description: "Sets the value of a dashboard item property. Use this resource
        in apps to store custom data against a dashboard item.  \n  \nA dashboard
        item enables an app to add user-specific information to a user dashboard.
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
        Permission to access Jira. However, to set a dashboard item property the user
        must be the owner of the dashboard. Note, users with the _Administer Jira_
        [global permission](href=) are considered owners of the System dashboard.
        \ \n  \nThe value of the request body must be a [valid](http://tools.ietf.org/html/rfc4627),
        non-empty JSON blob. The maximum length is 32768 bytes."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.setDashboardItemProperty_put
      x-api-path-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
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
      - Set
      - Dashboard
      - Item
      - Property
    delete:
      summary: Delete dashboard item property
      description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira. However, to delete a dashboard item
        property the user must be the owner of the dashboard. Note, users with the
        _Administer Jira_ [global permission](href=) are considered owners of the
        System dashboard."
      operationId: com.atlassian.jira.rest.v2.dashboard.DashboardItemPropertyResource.deleteDashboardItemProperty_delet
      x-api-path-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
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
    post:
      summary: Create issue field option
      description: |-
        Creates an option for a select list issue field.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.createIssueFieldOption_post
      x-api-path-slug: api2fieldfieldkeyoption-post
      parameters:
      - in: path
        name: fieldKey
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
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
    put:
      summary: Update issue field option
      description: |-
        Updates an option for a select list issue field. If the option does not exist, a new option is created.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.updateIssueFieldOption_put
      x-api-path-slug: api2fieldfieldkeyoptionoptionid-put
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: path
        name: optionId
        description: The ID of the option to be updated
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
    delete:
      summary: Delete issue field option
      description: |-
        Deletes an option from a select list issue field.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.deleteIssueFieldOption_delete
      x-api-path-slug: api2fieldfieldkeyoptionoptionid-delete
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: path
        name: optionId
        description: The ID of the option to be deleted
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
  /api/2/field/{fieldKey}/option/{optionId}/issue:
    delete:
      summary: Replace issue field option
      description: |-
        Deselects a select list issue field option in all issues that it has been selected in. A different option can be selected to replace the deselected option. The update can also be limited to a smaller set of issues by using a JQL query.

        This is an [asynchronous method](#async). The response object will contain a link to the long-running task. For example, _https://your-domain.atlassian.net/rest/api/2/task/10127_.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.replaceIssueFieldOption_delete
      x-api-path-slug: api2fieldfieldkeyoptionoptionidissue-delete
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: jql
        description: A JQL query that specifies the issues to be updated
      - in: path
        name: optionId
        description: The ID of the option to be deselected
      - in: query
        name: replaceWith
        description: The ID of the option that will replace the currently selected
          option
      responses:
        200:
          description: OK
      tags:
      - Replace
      - Issue
      - Field
      - Option
  /api/2/issue/properties/{propertyKey}:
    put:
      summary: Bulk set issue property
      description: |-
        Allows to set a property for all issues identified by a given filter. Only entities the user has permissions to edit will be updated.

        Currently the following filters are available:

        *   **entityIds** \- A list of issues to update. Only issues with ids from this list will be considered for updating. This is an optional filter, if not provided, then any editable issue that matches all other filters will be updated.
        *   **currentValue** \- If provided, then only issues with the property currently set to that value will be updated.
        *   **hasProperty** \- If true, then only existing properties will be updated. If false, then only issues that do not have any value associated with this property will be updated. If omitted, the property will be set on all issues, regardless of whether it previously existed or not.

        If more than one filter is given, then they are all joined with the logical "and", that is: only issues that satisfy all filters are updated. If no filters are provided at all, then the property will be updated on _all_ issues editable by the caller (i.e. issues in projects with the EDIT_ISSUES permission).

        If an invalid combination of filters is provided, an error will be returned by the API. For example, specifying the current value and "hasProperty" to "false" would never match any issues (as it would mean: update this property if the current value is something, oh, but only if there is no value at all) and is therefore not allowed.

        This method is [asynchronous](#async), meaning that it will not return the results immediately, instead creating a task to perform the requested update operation (unless preliminary validation, e.g. of the provided filter, fails).

        The operation is transactional: either all eligible issues are updated, or none (if there are any errors).
      operationId: com.atlassian.jira.rest.v2.property.IssuePropertyBulkUpdateResource.bulkSetIssueProperty_put
      x-api-path-slug: api2issuepropertiespropertykey-put
      parameters:
      - in: path
        name: propertyKey
        description: The key of the property to update
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Set
      - Issue
      - Property
    delete:
      summary: Bulk delete issue property
      description: Allows to delete a property from all issues identified by a given
        filter. Only entities the user has permissions to edit will be updated. See
        the [issue property bulk set endpoint documentation](#api-api-2-issue-properties-propertyKey-put)
        for more details.
      operationId: com.atlassian.jira.rest.v2.property.IssuePropertyBulkUpdateResource.bulkDeleteIssueProperty_delete
      x-api-path-slug: api2issuepropertiespropertykey-delete
      parameters:
      - in: path
        name: propertyKey
        description: The key of the property to delete
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Delete
      - Issue
      - Property
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
    put:
      summary: Edit issue
      description: "Edits the issue from a JSON representation.\n\nThe fields available
        for update can be determined using the **/rest/api/2/issue/{issueIdOrKey}/editmeta**
        resource.  \nIf a field is hidden from the Edit screen then it will not be
        returned by the editmeta resource. A field validation error will occur if
        such field is submitted in an edit request. However connect add-on with admin
        scope may override a screen security configuration.\n\nIf an issue cannot
        be edited in Jira because of its workflow status (for example the issue is
        closed), then you will not be able to edit it with this resource.\n\nField
        to be updated should appear either in `fields` or `update` request's body
        parameter, but not in both.  \nTo update a single sub-field of a complex field
        (e.g. timetracking) please use the `update` parameter of the edit operation.
        Using a `\"field_id\": field_value` construction in the `fields` parameter
        is a shortcut of \"set\" operation in the `update` parameter."
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.editIssue_put
      x-api-path-slug: api2issueissueidorkey-put
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to be updated
      - in: query
        name: notifyUsers
        description: Sends the notification email on issue update to all watchers
      - in: query
        name: overrideEditableFlag
        description: Updates the issue even if it is not editable (issue in status
          with jira
      - in: query
        name: overrideScreenSecurity
        description: Allows update of the fields that are hidden from the issues Edit
          screen
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Issue
    delete:
      summary: Delete issue
      description: |-
        Deletes an individual issue.

        If the issue has sub-tasks you must set the `deleteSubtasks=true` parameter to delete the issue. You cannot delete an issue without deleting its sub-tasks.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.deleteIssue_delete
      x-api-path-slug: api2issueissueidorkey-delete
      parameters:
      - in: query
        name: deleteSubtasks
        description: A `true` or `false` value indicating if sub-tasks should be deleted
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to be deleted
      responses:
        200:
          description: OK
      tags:
      - Issue
  /api/2/issue/{issueIdOrKey}/assignee:
    put:
      summary: Assign issue
      description: Assigns the issue to the user. Use this resource to assign issues
        for the users having "Assign Issue" permission, and not having the "Edit Issue"
        permission. If `name` body parameter is set to "-1" then automatic issue assignee
        is used. A `name` set to `null` will remove the assignee.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.assignIssue_put
      x-api-path-slug: api2issueissueidorkeyassignee-put
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to be updated
      responses:
        200:
          description: OK
      tags:
      - Assign
      - Issue
  /api/2/issue/{issueIdOrKey}/attachments:
    post:
      summary: Add attachment
      description: |-
        Add one or more attachments to an issue.

        This resource expects a multipart post. The media-type multipart/form-data is defined in RFC 1867. Most client libraries have classes that make dealing with multipart posts simple. For instance, in Java the Apache HTTP Components library provides a [MultiPartEntity](http://hc.apache.org/httpcomponents-client-ga/httpmime/apidocs/org/apache/http/entity/mime/MultipartEntity.html) that makes it simple to submit a multipart POST.

        In order to protect against XSRF attacks, because this method accepts multipart/form-data, it has XSRF protection on it. This means you must submit a header of X-Atlassian-Token: no-check with the request, otherwise it will be blocked.

        The name of the multipart/form-data parameter that contains attachments must be "file"

        A simple example to upload a file called "myfile.txt" to issue REST-123:

        curl -D- -u admin:admin -X POST -H "X-Atlassian-Token: no-check" -F "file=@myfile.txt" http://myhost/rest/api/2/issue/TEST-123/attachments
      operationId: com.atlassian.jira.rest.v2.issue.IssueAttachmentsResource.addAttachment_post
      x-api-path-slug: api2issueissueidorkeyattachments-post
      parameters:
      - in: path
        name: issueIdOrKey
        description: the issue that you want to add the attachments to
      responses:
        200:
          description: OK
      tags:
      - Attachment
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