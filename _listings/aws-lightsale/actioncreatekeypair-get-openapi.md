---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Create Key Pair
  version: 1.0.0
  description: Creates sn SSH key pair.
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