---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Get API Keys
  version: 1.0.0
  description: Gets the ApiKeys resource representing the set of ApiKey resources
    to identify clients for all of your APIs.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apikeys:
    get:
      summary: Get API Keys
      description: Gets the ApiKeys resource representing the set of ApiKey resources
        to identify clients for all of your APIs.
      operationId: apigatewayApi-keys
      x-api-path-slug: apikeys-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
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