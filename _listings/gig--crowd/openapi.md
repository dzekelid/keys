swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/key/{key}:
    get:
      summary: Get Request Key Key
      description: Get request key key.
      operationId: getApiV1RequestKeyKey
      x-api-path-slug: apiv1requestkeykey-get
      parameters:
      - in: path
        name: key
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Key
      - Key