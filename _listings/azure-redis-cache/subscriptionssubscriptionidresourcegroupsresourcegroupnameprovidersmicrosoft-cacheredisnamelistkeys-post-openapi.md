---
swagger: "2.0"
x-collection-name: Azure Redis Cache
x-complete: 0
info:
  title: Azure Redis Cache API Redis List Keys
  description: Retrieve a Redis cache's access keys. This operation requires write
    permission to the cache resource.
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Cache/Redis/{name}/listKeys:
    post:
      summary: Redis List Keys
      description: Retrieve a Redis cache's access keys. This operation requires write
        permission to the cache resource.
      operationId: Redis_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cacheredisnamelistkeys-post
      parameters:
      - in: path
        name: name
        description: The name of the Redis cache
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Redis Keys
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