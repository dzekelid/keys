---
name: Azure Media Services
x-slug: azure-media-services
description: Azure Media Services gives you broadcast-quality video streaming services
  to reach larger audiences on today&rsquo;s most popular mobile devices. Media Services
  enhances accessibility, distribution, and scalability, and makes it easy and cost-effective
  to stream content to your local and worldwide audiences&mdash;all while protecting
  your content.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/media-services-video-on-demand.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-media-services/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Media Services API Media Service List Keys
  x-api-slug: azure-media-services-api
  description: Lists the keys for a Media Service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/media-services-video-on-demand.png
  humanURL: https://azure.microsoft.com/en-us/services/media-services/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Media/mediaservices/{mediaServiceName}/listKeys
  tags: Media Service Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-media-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-mediamediaservicesmediaservicenamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-media-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-mediamediaservicesmediaservicenamelistkeys-post-openapi.md
- name: Azure Media Services API Media Service Sync Storage Keys
  x-api-slug: azure-media-services-api
  description: Synchronizes storage account keys for a storage account associated
    with the Media Service account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/media-services-video-on-demand.png
  humanURL: https://azure.microsoft.com/en-us/services/media-services/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Media/mediaservices/{mediaServiceName}/syncStorageKeys
  tags: Media Service Sync Storage Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-media-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-mediamediaservicesmediaservicenamesyncstoragekeys-post-openapi.md
- name: Azure Media Services API
  x-api-slug: azure-media-services-api
  description: Azure Media Services gives you broadcast-quality video streaming services
    to reach larger audiences on today&rsquo;s most popular mobile devices. Media
    Services enhances accessibility, distribution, and scalability, and makes it easy
    and cost-effective to stream content to your local and worldwide audiences&mdash;all
    while protecting your content.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/media-services-video-on-demand.png
  humanURL: https://azure.microsoft.com/en-us/services/media-services/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-media-services/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/media-services/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/media-services/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/media-services/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/media-services/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---