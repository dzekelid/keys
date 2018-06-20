---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Get Access Key Last Used
  version: 1.0.0
  description: Retrieves information about when the specified access key was last
    used.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateAccessKey:
    get:
      summary: Create Access Key
      description: |-
        Creates a new AWS secret access key and corresponding AWS access key ID for the
              specified user.
      operationId: createAccessKey
      x-api-path-slug: actioncreateaccesskey-get
      parameters:
      - in: query
        name: UserName
        description: The name of the IAM user that the new key will belong to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=DeleteAccessKey:
    get:
      summary: Delete Access Key
      description: Deletes the access key pair associated with the specified IAM user.
      operationId: deleteAccessKey
      x-api-path-slug: actiondeleteaccesskey-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The access key ID for the access key ID and secret access key
          you want to      delete
        type: string
      - in: query
        name: UserName
        description: The name of the user whose access key pair you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=GetAccessKeyLastUsed:
    get:
      summary: Get Access Key Last Used
      description: Retrieves information about when the specified access key was last
        used.
      operationId: getAccessKeyLastUsed
      x-api-path-slug: actiongetaccesskeylastused-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The identifier of an access key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
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