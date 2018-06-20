---
name: Azure Search
x-slug: azure-search
description: Azure Search is a fully-managed service for adding sophisticated search
  capabilities to web and mobile applications without the typical complexities of
  full-text search.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Search API Admin Keys Get
  x-api-slug: azure-search-api
  description: Gets the primary and secondary admin API keys for the specified Azure
    Search service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/listAdminKeys
  tags: Admin Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistadminkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistadminkeys-post-openapi.md
- name: Azure Search API Admin Keys Regenerate
  x-api-slug: azure-search-api
  description: Regenerates either the primary or secondary admin API key. You can
    only regenerate one key at a time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/regenerateAdminKey/{keyKind}
  tags: Admin Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenameregenerateadminkeykeykind-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenameregenerateadminkeykeykind-post-openapi.md
- name: Azure Search API Query Keys Create
  x-api-slug: azure-search-api
  description: Generates a new query key for the specified Search service. You can
    create up to 50 query keys per service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/createQueryKey/{name}
  tags: Query Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamecreatequerykeyname-post-openapi.md
- name: Azure Search API Query Keys List By Search Service
  x-api-slug: azure-search-api
  description: Returns the list of query API keys for the given Azure Search service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/listQueryKeys
  tags: Query Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamelistquerykeys-get-openapi.md
- name: Azure Search API Query Keys Delete
  x-api-slug: azure-search-api
  description: Deletes the specified query key. Unlike admin keys, query keys are
    not regenerated. The process for regenerating a query key is to delete and then
    recreate it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/deleteQueryKey/{key}
  tags: Query Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-searchsearchservicessearchservicenamedeletequerykeykey-delete-openapi.md
- name: Azure Search API
  x-api-slug: azure-search-api
  description: Azure Search is a fully-managed service for adding sophisticated search
    capabilities to web and mobile applications without the typical complexities of
    full-text search.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-search/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/search/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/search/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/search/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/search/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---