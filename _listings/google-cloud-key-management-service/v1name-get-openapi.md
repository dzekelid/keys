---
swagger: "2.0"
x-collection-name: Google Cloud Key Management Service
x-complete: 0
info:
  title: Google Cloud Key Management Service API Get Key
  description: Returns metadata for a given CryptoKeyVersion.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudkms.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    get:
      summary: Get Key
      description: Returns metadata for a given CryptoKeyVersion.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the CryptoKeyVersion to get
      responses:
        200:
          description: OK
      tags:
      - Key
    patch:
      summary: Update Key
      description: |-
        Update a CryptoKeyVersion's metadata.

        state may be changed between
        ENABLED and
        DISABLED using this
        method. See DestroyCryptoKeyVersion and RestoreCryptoKeyVersion to
        move between other states.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.patch
      x-api-path-slug: v1name-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Output only
      - in: query
        name: updateMask
        description: Required list of fields to be updated in this request
      responses:
        200:
          description: OK
      tags:
      - Key
  /v1/{name}:destroy:
    post:
      summary: Destroy Key
      description: |-
        Schedule a CryptoKeyVersion for destruction.

        Upon calling this method, CryptoKeyVersion.state will be set to
        DESTROY_SCHEDULED
        and destroy_time will be set to a time 24
        hours in the future, at which point the state
        will be changed to
        DESTROYED, and the key
        material will be irrevocably destroyed.

        Before the destroy_time is reached,
        RestoreCryptoKeyVersion may be called to reverse the process.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.destroy
      x-api-path-slug: v1namedestroy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the CryptoKeyVersion to destroy
      responses:
        200:
          description: OK
      tags:
      - Key
  /v1/{name}:restore:
    post:
      summary: Restore Key
      description: |-
        Restore a CryptoKeyVersion in the
        DESTROY_SCHEDULED,
        state.

        Upon restoration of the CryptoKeyVersion, state
        will be set to DISABLED,
        and destroy_time will be cleared.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.restore
      x-api-path-slug: v1namerestore-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the CryptoKeyVersion to restore
      responses:
        200:
          description: OK
      tags:
      - Key
  /v1/{parent}/cryptoKeys:
    get:
      summary: List Keys
      description: Lists CryptoKeys.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.list
      x-api-path-slug: v1parentcryptokeys-get
      parameters:
      - in: query
        name: pageSize
        description: Optional limit on the number of CryptoKeys to include in theresponse
      - in: query
        name: pageToken
        description: Optional pagination token, returned earlier viaListCryptoKeysResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Key
    post:
      summary: Create Key
      description: |-
        Create a new CryptoKey within a KeyRing.

        CryptoKey.purpose is required.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.create
      x-api-path-slug: v1parentcryptokeys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: cryptoKeyId
        description: Required
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
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