---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get dashboard item property keys
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
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