swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
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
  /?Action=DescribeKeyPairs:
    get:
      summary: Describe Key Pairs
      description: Describes one or more of your key pairs.
      operationId: describekeypairs
      x-api-path-slug: actiondescribekeypairs-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: KeyName
        description: A unique name for the key pair
        type: string
      - in: query
        name: PublicKeyMaterial
        description: The public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Paris
  /?Action=ImportKeyPair:
    get:
      summary: Import Key Pair
      description: Imports the public key from an RSA key pair that you created with
        a third-party tool.
      operationId: importkeypair
      x-api-path-slug: actionimportkeypair-get
      parameters:
      - in: query
        name: AllocationId
        description: The allocation ID of an Elastic IP address to associate with
          the NAT gateway
        type: string
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: SubnetId
        description: The subnet in which to create the NAT gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pair