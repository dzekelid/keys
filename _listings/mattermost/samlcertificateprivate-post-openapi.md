---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Upload private key
  description: |-
    Upload the private key to be used for encryption with your SAML configuration. This will also set the filename for the PrivateKeyFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /saml/certificate/private:
    post:
      summary: Upload private key
      description: |-
        Upload the private key to be used for encryption with your SAML configuration. This will also set the filename for the PrivateKeyFile setting in your `config.json`.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: upload-the-private-key-to-be-used-for-encryption-with-your-saml-configuration-this-will-also-set-the
      x-api-path-slug: samlcertificateprivate-post
      parameters:
      - in: formData
        name: certificate
        description: The private key file
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Private
      - Key
    delete:
      summary: Remove private key
      description: |-
        Delete the current private key being used with your SAML configuration. This will also disable encryption for SAML on your system as this key is required for that.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: delete-the-current-private-key-being-used-with-your-saml-configuration-this-will-also-disable-encryp
      x-api-path-slug: samlcertificateprivate-delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Private
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