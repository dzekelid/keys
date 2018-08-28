---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Remove keys from a property
  version: 1.0.0
  description: Remove keys from a property.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/{id}/keys/remove:
    delete:
      summary: Remove keys from a property
      description: Remove keys from a property.
      operationId: Property_RemoveKeysByidBykeyIds
      x-api-path-slug: apipropertyidkeysremove-delete
      parameters:
      - in: path
        name: id
        description: The property id
      - in: query
        name: keyIds
        description: The ids of the keys to remove
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Keys
      - From
      - Property
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