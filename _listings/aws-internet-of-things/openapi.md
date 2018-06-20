---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateKeysAndCertificate:
    get:
      summary: Create Keys And Certificate
      description: Creates a 2048-bit RSA key pair and issues an X.
      operationId: createKeysAndCertificate
      x-api-path-slug: actioncreatekeysandcertificate-get
      parameters:
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys And Certificates
---