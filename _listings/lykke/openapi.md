---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Client/keys/encodedmainkey:
    post:
      summary: Add API Client Keys Encodedmainkey
      description: Add api client keys encodedmainkey.
      operationId: ApiClientKeysEncodedmainkeyPost
      x-api-path-slug: apiclientkeysencodedmainkey-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Keys
      - Encodedmainkey
  /api/ClientKeys:
    post:
      summary: Add API Clientkeys
      description: Add api clientkeys.
      operationId: ApiClientKeysPost
      x-api-path-slug: apiclientkeys-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientkeys
---