swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
  /api/property/{id}/keys:
    get:
      summary: Get a list of keys for a property
      description: Get a list of keys for a property.
      operationId: Property_KeysByid
      x-api-path-slug: apipropertyidkeys-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Keysa
      - Property
  /api/property/{id}/keys/add:
    post:
      summary: Add keys for a property
      description: Add keys for a property.
      operationId: Property_AddKeysByidBykeysToAdd
      x-api-path-slug: apipropertyidkeysadd-post
      parameters:
      - in: path
        name: id
        description: The property id
      - in: body
        name: keysToAdd
        description: A collection of keys to add
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Keysa
      - Property
  /api/property/{id}/keys/checkout:
    put:
      summary: Checkout a collection of keys for a property
      description: Checkout a collection of keys for a property.
      operationId: Property_CheckoutKeysByidBycheckoutDetails
      x-api-path-slug: apipropertyidkeyscheckout-put
      parameters:
      - in: body
        name: checkoutDetails
        description: The details of the keys to checkout
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Collection
      - Of
      - Keysa
      - Property
  /api/property/{id}/keys/checkin:
    put:
      summary: Checkin a collection of keys for a property
      description: Checkin a collection of keys for a property.
      operationId: Property_CheckinKeysByidBycheckinDetails
      x-api-path-slug: apipropertyidkeyscheckin-put
      parameters:
      - in: body
        name: checkinDetails
        description: The details of the keys to checkin
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Collection
      - Of
      - Keysa
      - Property
  /api/negotiator/my/keys:
    get:
      summary: Return all Negotiator keys for the side bar display.
      description: Return all negotiator keys for the side bar display..
      operationId: Negotiator_KeysBypageSizeBypageNumberBycheckedOutOnly
      x-api-path-slug: apinegotiatormykeys-get
      parameters:
      - in: query
        name: checkedOutOnly
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Negotiator
      - Keysthe
      - Side
      - Bar
      - Display
  /api/agency/apikey:
    post:
      summary: Issues an API key for use with the simple role/search endpoints
      description: Issues an api key for use with the simple role/search endpoints.
      operationId: Agency_IssueApiKeyBysubjectId
      x-api-path-slug: apiagencyapikey-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subjectId
        description: The Id of the group to assign a key to
      responses:
        200:
          description: OK
      tags:
      - Issues
      - Keyuse
      - Simple
      - Role
      - Search
      - Endpoints
  /api/branch/checkkeycodesexist:
    get:
      summary: Check specified key codes exist in branch
      description: Check specified key codes exist in branch.
      operationId: Branch_CheckKeycodesExistBykeyCodes
      x-api-path-slug: apibranchcheckkeycodesexist-get
      parameters:
      - in: query
        name: keyCodes
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Check
      - Specified
      - Key
      - Codes
      - Exist
      - In
      - Branch
  /api/cache/Key:
    get:
      summary: Generate a guid for use as a key
      description: Generate a guid for use as a key.
      operationId: Cache_GenerateKey
      x-api-path-slug: apicachekey-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Guiduse
      - As
      - Key
  /api/cache/List/{listKey}:
    get:
      summary: Retrieves a list of objects stored in the cache system by its {listKey}
      description: Retrieves a list of objects stored in the cache system by its {listkey}.
      operationId: Cache_GetListBylistKey
      x-api-path-slug: apicachelistlistkey-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - List
      - Of
      - Objects
      - Stored
      - In
      - Cache
      - System
      - By
      - Its
      - ListKey
  /api/cache/List/{listKey}/Append:
    put:
      summary: Adds {itemToAppend} to the tail of an existing list, or creates a new
        list with the object in it.
      description: Adds {itemtoappend} to the tail of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_AppendToListByitemToAppendBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyappend-put
      parameters:
      - in: body
        name: itemToAppend
        description: The item to append
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToAppend
      - To
      - Tail
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/cache/List/{listKey}/Item:
    delete:
      summary: Removes a given item from the list.
      description: Removes a given item from the list..
      operationId: Cache_RemoveItemFromListByitemToRemoveBylistKey
      x-api-path-slug: apicachelistlistkeyitem-delete
      parameters:
      - in: body
        name: itemToRemove
        description: The item to remove
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Given
      - Item
      - From
      - List
  /api/cache/List/{listKey}/Pop:
    get:
      summary: Pops an items from the list head.
      description: Pops an items from the list head..
      operationId: Cache_PopFromListHeadBylistKey
      x-api-path-slug: apicachelistlistkeypop-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Pops
      - Items
      - From
      - List
      - Head
  /api/cache/List/{listKey}/Prepend:
    put:
      summary: Adds {itemToPrepend} to the head of an existing list, or creates a
        new list with the object in it.
      description: Adds {itemtoprepend} to the head of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_PrependToListByitemToPrependBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyprepend-put
      parameters:
      - in: body
        name: itemToPrepend
        description: The item to prepend
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToPrepend
      - To
      - Head
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/cache/{itemKey}:
    get:
      summary: Retrieves an object stored in the cache system by its {itemKey}
      description: Retrieves an object stored in the cache system by its {itemkey}.
      operationId: Cache_GetObjectByitemKey
      x-api-path-slug: apicacheitemkey-get
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - Object
      - Stored
      - In
      - Cache
      - System
      - By
      - Its
      - ItemKey
    put:
      summary: Stores the {objectToPersist} in the cache subsystem.
      description: Stores the {objecttopersist} in the cache subsystem..
      operationId: Cache_SetObjectByobjectToPersistByitemKeyBytimeToLive
      x-api-path-slug: apicacheitemkey-put
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: body
        name: objectToPersist
        description: The object to persist
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - Stores
      - ObjectToPersist
      - In
      - Cache
      - Subsystem
    delete:
      summary: Deletes the item stored at {itemKey}
      description: Deletes the item stored at {itemkey}.
      operationId: Cache_DeleteItemByitemKey
      x-api-path-slug: apicacheitemkey-delete
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Item
      - Stored
      - At
      - ItemKey