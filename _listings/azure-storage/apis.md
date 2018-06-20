---
name: Azure Storage
x-slug: azure-storage
description: Azure Storage offers non-relational data storage including Blob Storage,
  Table Storage, Queue Storage, and Files.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-storage/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Storage API Storage Accounts List Keys
  x-api-slug: azure-storage-api
  description: Lists the access keys for the specified storage account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/listKeys
  tags: Storage Accounts Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storagestorageaccountsaccountnamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-storage/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storagestorageaccountsaccountnamelistkeys-post-openapi.md
- name: Azure Storage API
  x-api-slug: azure-storage-api
  description: Azure Storage offers non-relational data storage including Blob Storage,
    Table Storage, Queue Storage, and Files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-storage.png
  humanURL: https://azure.microsoft.com/en-us/services/storage/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-storage/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/storage/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/storage/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/storage/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/storage/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---