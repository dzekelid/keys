---
swagger: "2.0"
x-collection-name: LaunchDarkly
x-complete: 0
info:
  title: Launch Darkly Create an environment
  description: Create an environment.
  termsOfService: https://launchdarkly.com/terms
  contact:
    name: LaunchDarkly Support
    url: https://support.launchdarkly.com
    email: support@launchdarkly.com
  version: 2.0.0
host: app.launchdarkly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /environments/{projectKey}:
    post:
      summary: Create an environment
      description: Create an environment.
      operationId: postEnvironment
      x-api-path-slug: environmentsprojectkey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Projects
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