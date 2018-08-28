---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 1
info:
  title: StorSimpleSeries8000ManagementClient
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/listKeys
  : post:
      summary: Storage Accounts List Keys
      description: Lists the access keys for the specified storage account.
      operationId: StorageAccounts_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storagestorageaccountsaccountnamelistkeys-post
      parameters:
      - in: path
        name: accountName
        description: The name of the storage account within the specified resource
          group
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Storage Accounts Keys
---