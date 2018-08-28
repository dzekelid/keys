---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Maker API AS keys retrieval
  description: Retrieves the list of AS keys existing within authorized scopes.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /asKeys:
    get:
      summary: AS keys retrieval
      description: Retrieves the list of AS keys existing within authorized scopes.
      operationId: retrieves-the-list-of-as-keys-existing-within-authorized-scopes
      x-api-path-slug: askeys-get
      parameters:
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 AS keys of
          the specified page
      responses:
        200:
          description: OK
      tags:
      - AS
      - Keys
      - Retrieval
    post:
      summary: AS key creation
      description: Creates a new AS key.
      operationId: creates-a-new-as-key
      x-api-path-slug: askeys-post
      parameters:
      - in: body
        name: asKey
        description: Contents of the AS key to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for an easy registration on
          a standalone Join Server
      responses:
        200:
          description: OK
      tags:
      - AS
      - Key
      - Creation
  /asKeys/{asKeyRef}:
    get:
      summary: AS key retrieval
      description: Retrieves the AS key corresponding to the provided AS key ref,
        if that AS key is within authorized scopes.
      operationId: retrieves-the-as-key-corresponding-to-the-provided-as-key-ref-if-that-as-key-is-within-authorized-sc
      x-api-path-slug: askeysaskeyref-get
      parameters:
      - in: path
        name: asKeyRef
        description: Ref of the AS key to retrieve
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for operations on a standalone
          Join Server
      responses:
        200:
          description: OK
      tags:
      - AS
      - Key
      - Retrieval
    put:
      summary: AS key update
      description: Updates the AS key corresponding to the provided asKey ref, if
        that AS key is within authorized scopes.
      operationId: updates-the-as-key-corresponding-to-the-provided-askey-ref-if-that-as-key-is-within-authorized-scope
      x-api-path-slug: askeysaskeyref-put
      parameters:
      - in: body
        name: asKey
        description: Contents of the AS key to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: asKeyRef
        description: Ref of the AS key to update
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for operations on a standalone
          Join Server
      responses:
        200:
          description: OK
      tags:
      - AS
      - Key
      - Update
    delete:
      summary: AS key deletion
      description: Deletes the AS key corresponding to the provided asKeyRef, if that
        AS key is within authorized scopes.
      operationId: deletes-the-as-key-corresponding-to-the-provided-askeyref-if-that-as-key-is-within-authorized-scopes
      x-api-path-slug: askeysaskeyref-delete
      parameters:
      - in: path
        name: asKeyRef
        description: Ref of the AS key to delete
      - in: query
        name: deviceToken
        description: Token provided by the manufacturer for operations on a standalone
          Join Server
      responses:
        200:
          description: OK
      tags:
      - AS
      - Key
      - Deletion
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