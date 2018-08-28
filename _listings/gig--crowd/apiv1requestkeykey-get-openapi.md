---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Request Key Key
  version: 1.0.0
  description: Get request key key.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/key/{key}:
    get:
      summary: Get Request Key Key
      description: Get request key key.
      operationId: getApiV1RequestKeyKey
      x-api-path-slug: apiv1requestkeykey-get
      parameters:
      - in: path
        name: key
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Key
      - Key
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