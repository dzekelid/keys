swagger: "2.0"
x-collection-name: MasterCard
x-complete: 1
info:
  title: MasterCard
  description: as-a-technology-company-in-the-global-payments-business-we-operate-the-worlds-fastest-payments-processing-network-connecting-consumers-financial-institutions-merchants-governments-and-businesses-in-more-than-210-countries-and-territories--mastercards-products-and-solutions-make-everyday-commerce-activities--such-as-shopping-traveling-running-a-business-and-managing-finances--easier-more-secure-and-more-efficient-for-everyone-
  version: 1.0.0
host: eas5stl0.mastercard.int:13046
basePath: /z0/core/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /block/{key}:
    get:
      summary: Get Block Key
      description: |-
        A specific block may be retrieved by its hash key. This is useful when
        navigating the chain.
      operationId: getBlockKey
      x-api-path-slug: blockkey-get
      parameters:
      - in: path
        name: key
        description: The hash key of the block to retrieve
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Block
      - Key
  /entry/{key}:
    get:
      summary: Get Entry Key
      description: |-
        Returns full detail of the value of the blockchain entry
        referenced by the specified key, if it has been previously recorded
        by your node's key-value store (database).
      operationId: getEntryKey
      x-api-path-slug: entrykey-get
      parameters:
      - in: path
        name: key
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Entry
      - Key