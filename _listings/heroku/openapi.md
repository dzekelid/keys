---
swagger: "2.0"
x-collection-name: Heroku
x-complete: 1
info:
  title: Heroku
  description: manage-your-heroku-apps-configs-collaborators--resources
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/keys:
    parameters:
      summary: Parameters User Keys
      description: Parameters user keys.
      operationId: parametersUserKeys
      x-api-path-slug: userkeys-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - User
      - Keys
    get:
      summary: Get User Keys
      description: List SSH keys.
      operationId: getUserKeys
      x-api-path-slug: userkeys-get
      parameters:
      - in: query
        name: Accept
        description: Content type
      - in: header
        name: Accept
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
    post:
      summary: Add User Keys
      description: Associate an SSH key with this account.
      operationId: postUserKeys
      x-api-path-slug: userkeys-post
      parameters:
      - in: query
        name: Accept
        description: Content type
      - in: header
        name: Accept
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
  /user/keys/{key}:
    parameters:
      summary: Parameters User Keys Key
      description: Parameters user keys key.
      operationId: parametersUserKeysKey
      x-api-path-slug: userkeyskey-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - User
      - Keys
      - Key
    delete:
      summary: Delete User Keys Key
      description: Remove an SSH key from this account.
      operationId: deleteUserKeysKey
      x-api-path-slug: userkeyskey-delete
      parameters:
      - in: query
        name: Accept
        description: Content type
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: key
        description: The username@hostname description field of the key
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
      - Key
---