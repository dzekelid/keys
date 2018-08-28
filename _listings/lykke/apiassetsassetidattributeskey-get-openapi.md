---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Assets Asset Attributes Key
  version: 1.0.0
  description: Get api assets asset attributes key.
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
  /api/Assets/{assetId}/attributes/{key}:
    get:
      summary: Get API Assets Asset Attributes Key
      description: Get api assets asset attributes key.
      operationId: ApiAssetsByAssetIdAttributesByKeyGet
      x-api-path-slug: apiassetsassetidattributeskey-get
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Asset
      - Attributes
      - Key
  /api/Client/dictionary/{key}:
    get:
      summary: Get API Client Dictionary Key
      description: Get api client dictionary key.
      operationId: ApiClientDictionaryByKeyGet
      x-api-path-slug: apiclientdictionarykey-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
    delete:
      summary: Delete API Client Dictionary Key
      description: Delete api client dictionary key.
      operationId: ApiClientDictionaryByKeyDelete
      x-api-path-slug: apiclientdictionarykey-delete
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
  /api/Dictionary/{key}:
    get:
      summary: Get API Dictionary Key
      description: Get api dictionary key.
      operationId: ApiDictionaryByKeyGet
      x-api-path-slug: apidictionarykey-get
      parameters:
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Dictionary
      - Key
  /api/PrivateWallet/key:
    post:
      summary: Add API Privatewallet Key
      description: Add api privatewallet key.
      operationId: ApiPrivateWalletKeyPost
      x-api-path-slug: apiprivatewalletkey-post
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
      - Privatewallet
      - Key
  /api/EncodedPrivateKey:
    post:
      summary: Add API Encodedprivatekey
      description: Add api encodedprivatekey.
      operationId: ApiEncodedPrivateKeyPost
      x-api-path-slug: apiencodedprivatekey-post
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
      - Encodedprivatekey
  /api/PrivateKeyOwnershipMsg:
    get:
      summary: Get API Privatekeyownershipmsg
      description: Get api privatekeyownershipmsg.
      operationId: ApiPrivateKeyOwnershipMsgGet
      x-api-path-slug: apiprivatekeyownershipmsg-get
      parameters:
      - in: query
        name: email
      - in: query
        name: partnerId
      responses:
        200:
          description: OK
      tags:
      - Privatekeyownershipmsg
    post:
      summary: Add API Privatekeyownershipmsg
      description: Add api privatekeyownershipmsg.
      operationId: ApiPrivateKeyOwnershipMsgPost
      x-api-path-slug: apiprivatekeyownershipmsg-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privatekeyownershipmsg
  /api/signatureVerificationToken/KeyConfirmation:
    get:
      summary: Get API Signatureverificationtoken Keyconfirmation
      description: Get api signatureverificationtoken keyconfirmation.
      operationId: ApiSignatureVerificationTokenKeyConfirmationGet
      x-api-path-slug: apisignatureverificationtokenkeyconfirmation-get
      parameters:
      - in: query
        name: email
      responses:
        200:
          description: OK
      tags:
      - Signatureverificationtoken
      - Keyconfirmation
    post:
      summary: Add API Signatureverificationtoken Keyconfirmation
      description: Add api signatureverificationtoken keyconfirmation.
      operationId: ApiSignatureVerificationTokenKeyConfirmationPost
      x-api-path-slug: apisignatureverificationtokenkeyconfirmation-post
      parameters:
      - in: body
        name: response
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Signatureverificationtoken
      - Keyconfirmation
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