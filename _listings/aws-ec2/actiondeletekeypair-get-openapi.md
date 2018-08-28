---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Delete Key Pair
  version: 1.0.0
  description: Deletes the specified key pair, by removing the public key from Amazon
    EC2.
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
      description: Creates a 2048-bit RSA key pair with the specified name.
      operationId: createkeypair
      x-api-path-slug: actioncreatekeypair-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: KeyName
        description: The name of the key pair
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pair
  /?Action=DeleteKeyPair:
    get:
      summary: Delete Key Pair
      description: Deletes the specified key pair, by removing the public key from
        Amazon EC2.
      operationId: deletekeypair
      x-api-path-slug: actiondeletekeypair-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: KeyName.N
        description: One or more key pair names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pair
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