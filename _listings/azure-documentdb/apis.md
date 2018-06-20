---
name: Azure DocumentDB
x-slug: azure-documentdb
description: Azure DocumentDB is a fully-managed NoSQL document database service that
  offers querying and transaction-processing over schema-free data, predictable and
  reliable performance, and rapid development.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-documentdb/apis.md
specificationVersion: "0.14"
apis:
- name: Azure DocumentDB API Database Accounts List Keys
  x-api-slug: azure-documentdb-api
  description: Lists the access keys for the specified Azure DocumentDB database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/listKeys
  tags: Database, Accounts, List, Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamelistkeys-post-openapi.md
- name: Azure DocumentDB API Database Accounts List Read Only Keys
  x-api-slug: azure-documentdb-api
  description: Lists the read-only access keys for the specified Azure DocumentDB
    database account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/readonlykeys
  tags: Database, Accounts, List, Read, Only, Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamereadonlykeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-documentdb/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamereadonlykeys-get-openapi.md
- name: Azure DocumentDB API
  x-api-slug: azure-documentdb-api
  description: Azure DocumentDB is a fully-managed NoSQL document database service
    that offers querying and transaction-processing over schema-free data, predictable
    and reliable performance, and rapid development.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-document-db-03-replicate.png
  humanURL: https://azure.microsoft.com/en-us/services/documentdb/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-documentdb/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/documentdb/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/documentdb/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/documentdb/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/documentdb/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---