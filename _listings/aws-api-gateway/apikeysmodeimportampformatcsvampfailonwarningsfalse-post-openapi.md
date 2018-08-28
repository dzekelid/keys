---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Imports One Or More API Keys
  version: 1.0.0
  description: Imports one or more API keys.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apikeys:
    get:
      summary: Get API Keys
      description: Gets the ApiKeys resource representing the set of ApiKey resources
        to identify clients for all of your APIs.
      operationId: apigatewayApi-keys
      x-api-path-slug: apikeys-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
    post:
      summary: Create Key
      description: Creates a new ApiKey resource to represent an API key.
      operationId: apikeyCreate
      x-api-path-slug: apikeys-post
      parameters:
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;enabled&quot;'
        type: string
      - in: header
        name: '&quot;name&quot;'
        type: string
      - in: header
        name: '&quot;restApiId&quot;'
        type: string
      - in: header
        name: '&quot;stageKeys&quot;'
        type: string
      - in: header
        name: '&quot;stageName&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: body
        name: restApiId
        description: A list of Stage resources that are associated with the ApiKey
          resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: stageName
        description: The stage name in the RestApi that the stage key references
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /apikeys/hzYAVO9Sg98nsNh65VfX81M84O2kyXVy6K1xwHD7:
    get:
      summary: Get API Key
      description: Gets the ApiKey resource with the specified key identifier.
      operationId: apikeyBy-key
      x-api-path-slug: apikeyshzyavo9sg98nsnh65vfx81m84o2kyxvy6k1xwhd7-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
    patch:
      summary: Apikey Update
      description: Changes an API key properties, including the description, enabled,
        and name properties.
      operationId: apikeyUpdate
      x-api-path-slug: apikeyshzyavo9sg98nsnh65vfx81m84o2kyxvy6k1xwhd7-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /apikeys?mode=import&amp;format=csv&amp;failonwarnings=false:
    post:
      summary: Imports One Or More API Keys
      description: Imports one or more API keys.
      operationId: apikeyImport
      x-api-path-slug: apikeysmodeimportampformatcsvampfailonwarningsfalse-post
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
      - Imports
  /apikeys/a2TprUZuzf2EKbbmMUotDaHYGg8kgxFypcarGved:
    delete:
      summary: Deletes An Api Key Resource
      description: Deletes an ApiKey resource.
      operationId: apikeyDelete
      x-api-path-slug: apikeysa2tpruzuzf2ekbbmmuotdahygg8kgxfypcargved-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key
      - Resource
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