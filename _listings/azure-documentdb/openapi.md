swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 1
info:
  title: DocumentDB
  description: azure-documentdb-database-service-resource-provider-rest-api
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/listKeys
  : post:
      summary: Database Accounts List Keys
      description: Lists the access keys for the specified Azure DocumentDB database
        account.
      operationId: DatabaseAccounts_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - List
      - Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/readonlykeys
  : get:
      summary: Database Accounts List Read Only Keys
      description: Lists the read-only access keys for the specified Azure DocumentDB
        database account.
      operationId: DatabaseAccounts_ListReadOnlyKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamereadonlykeys-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - List
      - Read
      - Only
      - Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/regenerateKey
  : post:
      summary: Database Accounts Regenerate Key
      description: Regenerates an access key for the specified Azure DocumentDB database
        account.
      operationId: DatabaseAccounts_RegenerateKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnameregeneratekey-post
      parameters:
      - in: body
        name: keyToRegenerate
        description: The name of the key to regenerate
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - Regenerate
      - Key