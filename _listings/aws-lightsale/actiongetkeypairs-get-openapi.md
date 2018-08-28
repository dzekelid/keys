---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Key Pairs
  version: 1.0.0
  description: Returns information about all key pairs in the user's account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateKeyPair:
    get:
      summary: Create Key Pair
      description: Creates sn SSH key pair.
      operationId: createKeyPair
      x-api-path-slug: actioncreatekeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name for your new key pair
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=DeleteKeyPair:
    get:
      summary: Delete Key Pair
      description: Deletes a specific SSH key pair.
      operationId: deleteKeyPair
      x-api-path-slug: actiondeletekeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name of the key pair to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=DownloadDefaultKeyPair:
    get:
      summary: Download Default Key Pair
      description: Downloads the default SSH key pair from the user's account.
      operationId: downloadDefaultKeyPair
      x-api-path-slug: actiondownloaddefaultkeypair-get
      parameters:
      - in: query
        name: privateKeyBase64
        description: A base64-encoded RSA private key
        type: string
      - in: query
        name: publicKeyBase64
        description: A base64-encoded public key of the ssh-rsa type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=GetKeyPair:
    get:
      summary: Get Key Pair
      description: Returns information about a specific key pair.
      operationId: getKeyPair
      x-api-path-slug: actiongetkeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name of the key pair for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=GetKeyPairs:
    get:
      summary: Get Key Pairs
      description: Returns information about all key pairs in the user's account.
      operationId: getKeyPairs
      x-api-path-slug: actiongetkeypairs-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get key pairs      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
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