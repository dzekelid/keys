swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Acknowledgements/{LogicbrokerKey}/Status:
    get:
      summary: Retrieve acknowledgement status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_GetAckStatus
      x-api-path-slug: apiv1acknowledgementslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Acknowledgement
      - Status
  /api/v1/Acknowledgements/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update acknowledgement status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_UpdateAckStatus
      x-api-path-slug: apiv1acknowledgementslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: path
        name: Status
        description: The Status
      responses:
        200:
          description: OK
      tags:
      - Acknowledgement
      - Status
  /api/v1/Invoices/{LogicbrokerKey}:
    get:
      summary: Returns the invoice with the specified key.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_GetInvoice
      x-api-path-slug: apiv1invoiceslogicbrokerkey-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The logicbroker key to search for
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Invoice
      - Specified
      - Key