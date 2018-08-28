---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Rotate Encryption Key
  version: 1.0.0
  description: Rotates the encryption keys for a cluster.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateSnapshotCopyGrant:
    get:
      summary: Create Snapshot Copy Grant
      description: |-
        Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key
                    (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a
                    destination region.
      operationId: createSnapshotCopyGrant
      x-api-path-slug: actioncreatesnapshotcopygrant-get
      parameters:
      - in: query
        name: KmsKeyId
        description: The unique identifier of the customer master key (CMK) to which
          to grant Amazon Redshift            permission
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RotateEncryptionKey:
    get:
      summary: Rotate Encryption Key
      description: Rotates the encryption keys for a cluster.
      operationId: rotateEncryptionKey
      x-api-path-slug: actionrotateencryptionkey-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster that you want to rotate
          the encryption keys            for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Encryption Keys
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