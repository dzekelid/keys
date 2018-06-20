---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 1
info:
  title: AWS API Gateway API
  version: 1.0.0
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
---