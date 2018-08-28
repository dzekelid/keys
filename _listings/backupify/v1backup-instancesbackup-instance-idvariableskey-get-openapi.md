---
swagger: "2.0"
x-collection-name: Backupify
x-complete: 0
info:
  title: Backupify Retrieve a specific variable by key for the specified backup_instance
  description: You can only retrieve variables for backup_instances you have access
    to
  version: 1.0.0
host: api.backupify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/backup_definitions/{backup_definition_id}/variables/{key}:
    get:
      summary: Retrieve a specific variable by key for the specified backup_definition
      description: You can only retrieve variables for backup_definitions you have
        access to
      operationId: getV1BackupDefinitionsBackupDefinitionVariablesKey
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariableskey-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve a variable for
      - in: path
        name: key
        description: The key, symbolic name, or identifier of the variable to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
      - Key
    put:
      summary: Update a specific variable by key for the specified backup_definition
      description: You can only update variables for backup_definitions you have access
        to. Additionally, it is not possible to update a variable's key. Requests
        including a modified key name will result in an error.
      operationId: putV1BackupDefinitionsBackupDefinitionVariablesKey
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariableskey-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve a variable for
      - in: path
        name: key
        description: The key, symbolic name, or identifier of the variable to update
      - in: formData
        name: name
        description: The human-friendly name to use for the variable
      - in: formData
        name: variable[default_value]
        description: A default value that can be used when no instance specific value
          is provided
      - in: formData
        name: variable[description]
        description: Description offering additional information or detail about the
          variable
      - in: formData
        name: variable[optional]
        description: Flag indicating whether this variable is optional or if a value
          is required
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
      - Key
  /v1/backup_instances/{backup_instance_id}/variables/{key}:
    get:
      summary: Retrieve a specific variable by key for the specified backup_instance
      description: You can only retrieve variables for backup_instances you have access
        to
      operationId: getV1BackupInstancesBackupInstanceVariablesKey
      x-api-path-slug: v1backup-instancesbackup-instance-idvariableskey-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve a variable for
      - in: path
        name: key
        description: The key of the variable to retrieve as defined by the backup_definition
          of the specified backup_instance
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Variables
      - Key
    put:
      summary: Update the value of a variable by key for the specified backup_instance
      description: You can only alter variables for backup_instances you have access
        to manage
      operationId: putV1BackupInstancesBackupInstanceVariablesKey
      x-api-path-slug: v1backup-instancesbackup-instance-idvariableskey-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to update a variable for
      - in: path
        name: key
        description: The key of the variable to update as defined by the backup_definition
          of the specified backup_instance
      - in: formData
        name: variable[value]
        description: The updated data to store at the specified key
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Variables
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