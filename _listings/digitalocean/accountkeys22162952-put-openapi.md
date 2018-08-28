---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean Update a Key
  description: To update the name of an SSH key, send a PUT request to either /v2/account/keys/$SSH_KEY_ID
    or /v2/account/keys/$SSH_KEY_FINGERPRINT. Set the "name" attribute to the new
    name you want to use.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/keys:
    get:
      summary: List all Keys
      description: "To list all of the keys in your account, send a GET request to
        /v2/account/keys.\r\n\r\nThe response will be a JSON object with a key set
        to _ssh_keys_."
      operationId: AccountKeysGet
      x-api-path-slug: accountkeys-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Keys
    post:
      summary: Create a new Key
      description: "To add a new SSH public key to your DigitalOcean account, send
        a POST request to /v2/account/keys. Set the \"name\" attribute to the name
        you wish to use and the \"public_key\" attribute to a string of the full public
        key you are adding.\n\nThe response body will be a JSON object with a key
        set to ssh_key. The value will be the complete generated key object. This
        will have the standard key attributes:\n\nName\tType\tDescription\nid\tinteger\tThis
        is a unique identification number for the key. This can be used to reference
        a specific SSH key when you wish to embed a key into a Droplet.\nfingerprint\tstring\tThis
        attribute contains the fingerprint value that is generated from the public
        key. This is a unique identifier that will differentiate it from other keys
        using a format that SSH recognizes.\npublic_key\tstring\tThis attribute contains
        the entire public key string that was uploaded. This is what is embedded into
        the root user's authorized_keys file if you choose to include this SSH key
        during Droplet creation.\nname\tstring\tThis is the human-readable display
        name for the given SSH key. This is used to easily identify the SSH keys when
        they are displayed."
      operationId: AccountKeysPost
      x-api-path-slug: accountkeys-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - New
      - Key
  /account/keys/22162952:
    get:
      summary: Retrieve an existing Key
      description: "To show information about a key, send a GET request to /v2/account/keys/$KEY_ID
        or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nThe response will be a JSON object
        with a key called _ssh_key_."
      operationId: AccountKeys22162952Get
      x-api-path-slug: accountkeys22162952-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Existing
      - Key
    put:
      summary: Update a Key
      description: To update the name of an SSH key, send a PUT request to either
        /v2/account/keys/$SSH_KEY_ID or /v2/account/keys/$SSH_KEY_FINGERPRINT. Set
        the "name" attribute to the new name you want to use.
      operationId: AccountKeys22162952Put
      x-api-path-slug: accountkeys22162952-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Key
    delete:
      summary: Destroy a Key
      description: "To destroy a public SSH key that you have in your account, send
        a DELETE request to /v2/account/keys/$KEY_ID or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nA
        204 status will be returned, indicating that the action was successful and
        that the response body is empty."
      operationId: AccountKeys22162952Delete
      x-api-path-slug: accountkeys22162952-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Destroy
      - Key
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