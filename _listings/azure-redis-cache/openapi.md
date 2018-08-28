---
swagger: "2.0"
x-collection-name: Azure Redis Cache
x-complete: 1
info:
  title: RedisManagementClient
  description: rest-api-for-azure-redis-cache-service-
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
---