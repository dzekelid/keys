---
name: Azure Redis Cache
x-slug: azure-redis-cache
description: Azure Redis Cache is based on the popular open source Redis cache. It
  gives you access to a secure, dedicated Redis cache, managed by Microsoft and accessible
  from any application within Azure.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-redis-cache-performance.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-redis-cache/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Redis Cache API Redis List Keys
  x-api-slug: azure-redis-cache-api
  description: Retrieve a Redis cache's access keys. This operation requires write
    permission to the cache resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-redis-cache-performance.png
  humanURL: https://azure.microsoft.com/en-us/services/cache/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Cache/Redis/{name}/listKeys
  tags: Redis Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-redis-cache/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cacheredisnamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-redis-cache/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cacheredisnamelistkeys-post-openapi.md
- name: Azure Redis Cache API
  x-api-slug: azure-redis-cache-api
  description: Azure Redis Cache is based on the popular open source Redis cache.
    It gives you access to a secure, dedicated Redis cache, managed by Microsoft and
    accessible from any application within Azure.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-redis-cache-performance.png
  humanURL: https://azure.microsoft.com/en-us/services/cache/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-redis-cache/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/redis-cache/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/cache/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/cache/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/cache/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---