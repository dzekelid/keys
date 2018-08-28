---
swagger: "2.0"
x-collection-name: Azure Media Services
x-complete: 1
info:
  title: MediaServicesManagementClient
  description: media-services-resource-management-apis-
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Media/mediaservices/{mediaServiceName}/listKeys
  : post:
      summary: Media Service List Keys
      description: Lists the keys for a Media Service.
      operationId: MediaService_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-mediamediaservicesmediaservicenamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Media Service Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Media/mediaservices/{mediaServiceName}/syncStorageKeys
  : post:
      summary: Media Service Sync Storage Keys
      description: Synchronizes storage account keys for a storage account associated
        with the Media Service account.
      operationId: MediaService_SyncStorageKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-mediamediaservicesmediaservicenamesyncstoragekeys-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: SyncStorageKeysInput
        description: Properties needed to synchronize the keys for a storage account
          to the Media Service
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Media Service Sync Storage Keys
---