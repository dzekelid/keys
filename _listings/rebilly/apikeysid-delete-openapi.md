---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Delete api key
  description: Delete api key with predefined identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-keys:
    get:
      summary: Retrieve a list of api keys
      description: Retrieve a list of api keys
      operationId: retrieve-a-list-of-api-keys
      x-api-path-slug: apikeys-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Api
      - Keys
    post:
      summary: Create an api key
      description: Create an api key
      operationId: create-an-api-key
      x-api-path-slug: apikeys-post
      parameters:
      - in: body
        name: body
        description: ApiKey resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Api
      - Key
  /api-keys/{id}:
    delete:
      summary: Delete api key
      description: Delete api key with predefined identifier string
      operationId: delete-api-key-with-predefined-identifier-string
      x-api-path-slug: apikeysid-delete
      responses:
        200:
          description: OK
      tags:
      - Api
      - Key
    get:
      summary: Retrieve api key
      description: Retrieve api key with specified identifier string
      operationId: retrieve-api-key-with-specified-identifier-string
      x-api-path-slug: apikeysid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Api
      - Key
    put:
      summary: Create or update api key with predefined ID
      description: Create or update api key with predefined identifier string
      operationId: create-or-update-api-key-with-predefined-identifier-string
      x-api-path-slug: apikeysid-put
      parameters:
      - in: body
        name: body
        description: ApiKey resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Api
      - Key
      - Predefined
      - ID
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