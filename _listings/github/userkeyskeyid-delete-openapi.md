---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Delete User Keys Key
  description: Delete a public key. Removes a public key. Requires that you are authenticated
    via Basic Auth or via OAuth with at least admin:public_key scope.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/keys:
    get:
      summary: Get Repos Owner Repo Keys
      description: Get list of keys.
      operationId: get-list-of-keys
      x-api-path-slug: reposownerrepokeys-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Keys
    post:
      summary: Add Repos Owner Repo Keys
      description: Create a key.
      operationId: create-a-key
      x-api-path-slug: reposownerrepokeys-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Keys
  /repos/{owner}/{repo}/keys/{keyId}:
    delete:
      summary: Delete Repos Owner Repo Keys Key
      description: Delete a key.
      operationId: delete-a-key
      x-api-path-slug: reposownerrepokeyskeyid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: keyId
        description: Id of key
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Keys
      - Key
    get:
      summary: Get Repos Owner Repo Keys Key
      description: Get a key
      operationId: get-a-key
      x-api-path-slug: reposownerrepokeyskeyid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: keyId
        description: Id of key
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Keys
      - Key
  /user/keys:
    get:
      summary: Get User Keys
      description: |-
        List your public keys.
        Lists the current user's keys. Management of public keys via the API requires
        that you are authenticated through basic auth, or OAuth with the 'user', 'write:public_key' scopes.
      operationId: list-your-public-keyslists-the-current-users-keys-management-of-public-keys-via-the-api-requiresthat
      x-api-path-slug: userkeys-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
    post:
      summary: Add User Keys
      description: Create a public key.
      operationId: create-a-public-key
      x-api-path-slug: userkeys-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
  /user/keys/{keyId}:
    delete:
      summary: Delete User Keys Key
      description: Delete a public key. Removes a public key. Requires that you are
        authenticated via Basic Auth or via OAuth with at least admin:public_key scope.
      operationId: delete-a-public-key-removes-a-public-key-requires-that-you-are-authenticated-via-basic-auth-or-via-o
      x-api-path-slug: userkeyskeyid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: keyId
        description: ID of key
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
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