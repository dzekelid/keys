---
swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 0
info:
  title: AWS Key Management Service API Cancel Key Deletion
  version: 1.0.0
  description: Cancels the deletion of a customer master key (CMK).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelKeyDeletion:
    get:
      summary: Cancel Key Deletion
      description: Cancels the deletion of a customer master key (CMK).
      operationId: cancelKeyDeletion
      x-api-path-slug: actioncancelkeydeletion-get
      parameters:
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) for which
          to cancel      deletion
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
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