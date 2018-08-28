---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_key_references
  description: get_key_references
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_key_references:
    get:
      summary: get_key_references
      description: get_key_references
      operationId: get-key-references
      x-api-path-slug: get-key-references-get
      parameters:
      - in: query
        name: key
        description: key
      responses:
        200:
          description: OK
      tags:
      - Get
      - Key
      - References
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