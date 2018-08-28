---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Users Keys
  version: 1.0.0
  description: Get the SSH keys of a specified user. Available only for admins.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/keys:
    get:
      summary: Get Projects Keys
      description: Get a specific project's deploy keys
      operationId: getV3ProjectsIdKeys
      x-api-path-slug: v3projectsidkeys-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
    post:
      summary: Post Projects Keys
      description: Add new deploy key to currently authenticated user
      operationId: postV3ProjectsIdKeys
      x-api-path-slug: v3projectsidkeys-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: formData
        name: key
        description: The new deploy key
      - in: formData
        name: title
        description: The name of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
  /v3/projects/{id}/keys/{key_id}:
    get:
      summary: Get Projects Keys Key
      description: Get projects keys key.
      operationId: getV3ProjectsIdKeysKeyId
      x-api-path-slug: v3projectsidkeyskey-id-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
    delete:
      summary: Delete Projects Keys Key
      description: Delete deploy key for a project
      operationId: deleteV3ProjectsIdKeysKeyId
      x-api-path-slug: v3projectsidkeyskey-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
  /v3/projects/{id}/keys/{key_id}/enable:
    post:
      summary: Post Projects Keys Key Enable
      description: This feature was added in GitLab 8.11
      operationId: postV3ProjectsIdKeysKeyIdEnable
      x-api-path-slug: v3projectsidkeyskey-idenable-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
      - Enable
  /v3/projects/{id}/keys/{key_id}/disable:
    delete:
      summary: Delete Projects Keys Key Disable
      description: This feature was added in GitLab 8.11
      operationId: deleteV3ProjectsIdKeysKeyIdDisable
      x-api-path-slug: v3projectsidkeyskey-iddisable-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
      - Disable
  /v3/projects/{id}/deploy_keys:
    get:
      summary: Get Projects Deploy Keys
      description: Get a specific project's deploy keys
      operationId: getV3ProjectsIdDeployKeys
      x-api-path-slug: v3projectsiddeploy-keys-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
    post:
      summary: Post Projects Deploy Keys
      description: Add new deploy key to currently authenticated user
      operationId: postV3ProjectsIdDeployKeys
      x-api-path-slug: v3projectsiddeploy-keys-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: formData
        name: key
        description: The new deploy key
      - in: formData
        name: title
        description: The name of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
  /v3/projects/{id}/deploy_keys/{key_id}:
    get:
      summary: Get Projects Deploy Keys Key
      description: Get projects deploy keys key.
      operationId: getV3ProjectsIdDeployKeysKeyId
      x-api-path-slug: v3projectsiddeploy-keyskey-id-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
    delete:
      summary: Delete Projects Deploy Keys Key
      description: Delete projects deploy keys key.
      operationId: deleteV3ProjectsIdDeployKeysKeyId
      x-api-path-slug: v3projectsiddeploy-keyskey-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
  /v3/projects/{id}/deploy_keys/{key_id}/enable:
    post:
      summary: Post Projects Deploy Keys Key Enable
      description: This feature was added in GitLab 8.11
      operationId: postV3ProjectsIdDeployKeysKeyIdEnable
      x-api-path-slug: v3projectsiddeploy-keyskey-idenable-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
      - Enable
  /v3/projects/{id}/deploy_keys/{key_id}/disable:
    delete:
      summary: Delete Projects Deploy Keys Key Disable
      description: Delete projects deploy keys key disable.
      operationId: deleteV3ProjectsIdDeployKeysKeyIdDisable
      x-api-path-slug: v3projectsiddeploy-keyskey-iddisable-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
      - Disable
  /v3/keys/{id}:
    get:
      summary: Get Keys
      description: Get single ssh key by id. Only available to admin users
      operationId: getV3KeysId
      x-api-path-slug: v3keysid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Keys
  /v3/users/{id}/keys:
    post:
      summary: Post Users Keys
      description: Add an SSH key to a specified user. Available only for admins.
      operationId: postV3UsersIdKeys
      x-api-path-slug: v3usersidkeys-post
      parameters:
      - in: path
        name: id
        description: The ID of the user
      - in: formData
        name: key
        description: The new SSH key
      - in: formData
        name: title
        description: The title of the new SSH key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Keys
    get:
      summary: Get Users Keys
      description: Get the SSH keys of a specified user. Available only for admins.
      operationId: getV3UsersIdKeys
      x-api-path-slug: v3usersidkeys-get
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
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