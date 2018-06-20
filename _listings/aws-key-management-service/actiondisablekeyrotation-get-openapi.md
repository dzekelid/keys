---
swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 0
info:
  title: AWS Key Management Service API Disable Key Rotation
  version: 1.0.0
  description: Disables rotation of the specified key.
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
  /?Action=CreateKey:
    get:
      summary: Create Key
      description: Creates a customer master key (CMK).
      operationId: createKey
      x-api-path-slug: actioncreatekey-get
      parameters:
      - in: query
        name: BypassPolicyLockoutSafetyCheck
        description: A flag to indicate whether to bypass the key policy lockout safety
          check
        type: string
      - in: query
        name: Description
        description: A description of the CMK
        type: string
      - in: query
        name: KeyUsage
        description: The intended use of the CMK
        type: string
      - in: query
        name: Origin
        description: The source of the CMKs key material
        type: string
      - in: query
        name: Policy
        description: The key policy to attach to the CMK
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=DeleteImportedKeyMaterial:
    get:
      summary: Delete Imported Key Material
      description: |-
        Deletes key material that you previously imported and makes the specified customer
              master key (CMK) unusable.
      operationId: deleteImportedKeyMaterial
      x-api-path-slug: actiondeleteimportedkeymaterial-get
      parameters:
      - in: query
        name: KeyId
        description: The identifier of the CMK whose key material to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=DescribeKey:
    get:
      summary: Describe Key
      description: Provides detailed information about the specified customer master
        key.
      operationId: describeKey
      x-api-path-slug: actiondescribekey-get
      parameters:
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=DisableKey:
    get:
      summary: Disable Key
      description: |-
        Sets the state of a customer master key (CMK) to disabled, thereby preventing its use
              for cryptographic operations.
      operationId: disableKey
      x-api-path-slug: actiondisablekey-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=DisableKeyRotation:
    get:
      summary: Disable Key Rotation
      description: Disables rotation of the specified key.
      operationId: disableKeyRotation
      x-api-path-slug: actiondisablekeyrotation-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
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