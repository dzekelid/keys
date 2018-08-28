---
swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 0
info:
  title: AWS Key Management Service API Get Key Rotation Status
  version: 1.0.0
  description: |-
    Retrieves a Boolean value that indicates whether key rotation is enabled for the
          specified key.
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
  /?Action=EnableKey:
    get:
      summary: Enable Key
      description: Marks a key as enabled, thereby permitting its use.
      operationId: enableKey
      x-api-path-slug: actionenablekey-get
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
  /?Action=EnableKeyRotation:
    get:
      summary: Enable Key Rotation
      description: Enables rotation of the specified customer master key.
      operationId: enableKeyRotation
      x-api-path-slug: actionenablekeyrotation-get
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
  /?Action=GenerateDataKey:
    get:
      summary: Generate Data Key
      description: |-
        Returns a data encryption key that you can use in your application to encrypt
              data locally.
      operationId: generateDataKey
      x-api-path-slug: actiongeneratedatakey-get
      parameters:
      - in: query
        name: EncryptionContext
        description: A set of key-value pairs that represents additional authenticated
          data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK under which to generate and encrypt
          the data encryption      key
        type: string
      - in: query
        name: KeySpec
        description: The length of the data encryption key
        type: string
      - in: query
        name: NumberOfBytes
        description: The length of the data encryption key in bytes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GenerateDataKeyWithoutPlaintext:
    get:
      summary: Generate Data Key Without Plaintext
      description: Returns a data encryption key encrypted under a customer master
        key (CMK).
      operationId: generateDataKeyWithoutPlaintext
      x-api-path-slug: actiongeneratedatakeywithoutplaintext-get
      parameters:
      - in: query
        name: EncryptionContext
        description: A set of key-value pairs that represents additional authenticated
          data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK under which to generate and encrypt
          the data encryption      key
        type: string
      - in: query
        name: KeySpec
        description: The length of the data encryption key
        type: string
      - in: query
        name: NumberOfBytes
        description: The length of the data encryption key in bytes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GetKeyRotationStatus:
    get:
      summary: Get Key Rotation Status
      description: |-
        Retrieves a Boolean value that indicates whether key rotation is enabled for the
              specified key.
      operationId: getKeyRotationStatus
      x-api-path-slug: actiongetkeyrotationstatus-get
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
  /?Action=ImportKeyMaterial:
    get:
      summary: Import Key Material
      description: |-
        Imports key material into an AWS KMS customer master key (CMK) from your existing key
              management infrastructure.
      operationId: importKeyMaterial
      x-api-path-slug: actionimportkeymaterial-get
      parameters:
      - in: query
        name: EncryptedKeyMaterial
        description: The encrypted key material to import
        type: string
      - in: query
        name: ExpirationModel
        description: Specifies whether the key material expires
        type: string
      - in: query
        name: ImportToken
        description: The import token that you received in the response to a previous
          GetParametersForImport request
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK to import the key material into
        type: string
      - in: query
        name: ValidTo
        description: The time at which the imported key material expires
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=ListKeys:
    get:
      summary: List Keys
      description: Lists the customer master keys.
      operationId: listKeys
      x-api-path-slug: actionlistkeys-get
      parameters:
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=PutKeyPolicy:
    get:
      summary: Put Key Policy
      description: Attaches a key policy to the specified customer master key (CMK).
      operationId: putKeyPolicy
      x-api-path-slug: actionputkeypolicy-get
      parameters:
      - in: query
        name: BypassPolicyLockoutSafetyCheck
        description: A flag to indicate whether to bypass the key policy lockout safety
          check
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      - in: query
        name: Policy
        description: The key policy to attach to the CMK
        type: string
      - in: query
        name: PolicyName
        description: The name of the key policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=ScheduleKeyDeletion:
    get:
      summary: Schedule Key Deletion
      description: Schedules the deletion of a customer master key (CMK).
      operationId: scheduleKeyDeletion
      x-api-path-slug: actionschedulekeydeletion-get
      parameters:
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) to delete
        type: string
      - in: query
        name: PendingWindowInDays
        description: The waiting period, specified in number of days
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=UpdateKeyDescription:
    get:
      summary: Update Key Description
      description: Updates the description of a customer master key (CMK).
      operationId: updateKeyDescription
      x-api-path-slug: actionupdatekeydescription-get
      parameters:
      - in: query
        name: Description
        description: New description for the CMK
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GetKeyPolicy:
    get:
      summary: Get Key Policy
      description: Retrieves a policy attached to the specified key.
      operationId: getKeyPolicy
      x-api-path-slug: actiongetkeypolicy-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      - in: query
        name: PolicyName
        description: String that contains the name of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Policies
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