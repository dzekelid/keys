---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 0
info:
  title: Azure Storage API Storage Accounts List Keys
  version: 1.0.0
  description: Lists the access keys for the specified storage account.
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