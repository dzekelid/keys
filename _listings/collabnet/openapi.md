swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userid}/authorization-keys:
    post:
      summary: Sets authorization keys by user id
      description: Sets authorization keys by user id.
      operationId: setAuthorizationKeysById
      x-api-path-slug: usersuseridauthorizationkeys-post
      parameters:
      - in: body
        name: body
        description: Authorization keys
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Authorization
      - Keys
      - By
      - User
    get:
      summary: Gets authorization keys by user id
      description: Gets authorization keys by user id.
      operationId: getAuthorizationKeysById
      x-api-path-slug: usersuseridauthorizationkeys-get
      parameters:
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Authorization
      - Keys
      - By
      - User
  /users/by-username/{username}/authorization-keys:
    post:
      summary: Sets authorization keys by username
      description: Sets authorization keys by username.
      operationId: setAuthorizationKeys
      x-api-path-slug: usersbyusernameusernameauthorizationkeys-post
      parameters:
      - in: body
        name: body
        description: Authorization keys
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Authorization
      - Keys
      - By
      - Username
    get:
      summary: Gets authorization keys by username
      description: Gets authorization keys by username.
      operationId: getAuthorizationKeysByUsername
      x-api-path-slug: usersbyusernameusernameauthorizationkeys-get
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Authorization
      - Keys
      - By
      - Username
  /server/licensekey:
    put:
      summary: Sets/Updates license key
      description: Sets/updates license key.
      operationId: enterLicenseKey
      x-api-path-slug: serverlicensekey-put
      parameters:
      - in: body
        name: body
        description: License key
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - License
      - Key