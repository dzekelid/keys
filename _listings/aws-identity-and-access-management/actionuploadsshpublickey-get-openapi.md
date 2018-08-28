---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Upload S S H Public Key
  version: 1.0.0
  description: Uploads an SSH public key and associates it with the specified IAM
    user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetContextKeysForCustomPolicy:
    get:
      summary: Get Context Keys For Custom Policy
      description: Gets a list of all of the context keys referenced in the input
        policies.
      operationId: getContextKeysForCustomPolicy
      x-api-path-slug: actiongetcontextkeysforcustompolicy-get
      parameters:
      - in: query
        name: PolicyInputList.member.N
        description: A list of policies for which you want the list of context keys
          referenced in those      policies
        type: string
      responses:
        200:
          description: OK
      tags:
      - Context Keys For Custom Policies
  /?Action=GetContextKeysForPrincipalPolicy:
    get:
      summary: Get Context Keys For Principal Policy
      description: |-
        Gets a list of all of the context keys referenced in all of the IAM policies attached
              to the specified IAM entity.
      operationId: getContextKeysForPrincipalPolicy
      x-api-path-slug: actiongetcontextkeysforprincipalpolicy-get
      parameters:
      - in: query
        name: PolicyInputList.member.N
        description: An optional list of additional policies for which you want the
          list of context keys      that are referenced
        type: string
      - in: query
        name: PolicySourceArn
        description: The ARN of a user, group, or role whose policies contain the
          context keys that you want      listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Context Keys For Principal Policies
  /?Action=ListAccessKeys:
    get:
      summary: List Access Keys
      description: Returns information about the access key IDs associated with the
        specified IAM user.
      operationId: listAccessKeys
      x-api-path-slug: actionlistaccesskeys-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=ListSSHPublicKeys:
    get:
      summary: List S S H Public Keys
      description: Returns information about the SSH public keys associated with the
        specified IAM user.
      operationId: listSSHPublicKeys
      x-api-path-slug: actionlistsshpublickeys-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to list SSH public keys for
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Keys
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
  /?Action=UpdateAccessKey:
    get:
      summary: Update Access Key
      description: Changes the status of the specified access key from Active to Inactive,
        or vice versa.
      operationId: updateAccessKey
      x-api-path-slug: actionupdateaccesskey-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The access key ID of the secret access key you want to update
        type: string
      - in: query
        name: Status
        description: The status you want to assign to the secret access key
        type: string
      - in: query
        name: UserName
        description: The name of the user whose key you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=DeleteSSHPublicKey:
    get:
      summary: Delete S S H Public Key
      description: Deletes the specified SSH public key.
      operationId: deleteSSHPublicKey
      x-api-path-slug: actiondeletesshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
  /?Action=GetSSHPublicKey:
    get:
      summary: Get S S H Public Key
      description: Retrieves the specified SSH public key, including metadata about
        the key.
      operationId: getSSHPublicKey
      x-api-path-slug: actiongetsshpublickey-get
      parameters:
      - in: query
        name: Encoding
        description: Specifies the public key encoding format to use in the response
        type: string
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
  /?Action=UpdateSSHPublicKey:
    get:
      summary: Update S S H Public Key
      description: Sets the status of an IAM user's SSH public key to active or inactive.
      operationId: updateSSHPublicKey
      x-api-path-slug: actionupdatesshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: Status
        description: The status to assign to the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Keys
  /?Action=UploadSSHPublicKey:
    get:
      summary: Upload S S H Public Key
      description: Uploads an SSH public key and associates it with the specified
        IAM user.
      operationId: uploadSSHPublicKey
      x-api-path-slug: actionuploadsshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyBody
        description: The SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to associate the SSH public key with
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
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