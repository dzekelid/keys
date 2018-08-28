---
name: Azure Notification Hubs
x-slug: azure-notification-hubs
description: Azure Notification Hubs provide an easy-to-use, multi-platform, scaled-out
  push engine. With a single cross-platform API call, you can easily send targeted
  and personalized push notifications to any mobile platform from any cloud or on-premises
  backend.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Notification Hubs API Namespaces List Keys
  x-api-slug: azure-notification-hubs-api
  description: Gets the Primary and Secondary ConnectionStrings to the namespace
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/listKeys
  tags: Namespaces Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenameauthorizationrulesauthorizationrulenamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenameauthorizationrulesauthorizationrulenamelistkeys-post-openapi.md
- name: Azure Notification Hubs API Namespaces Regenerate Keys
  x-api-slug: azure-notification-hubs-api
  description: Regenerates the Primary/Secondary Keys to the Namespace Authorization
    Rule
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/regenerateKeys
  tags: Namespaces Regenerate Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenameauthorizationrulesauthorizationrulenameregeneratekeys-post-openapi.md
- name: Azure Notification Hubs API Notification Hubs List Keys
  x-api-slug: azure-notification-hubs-api
  description: Gets the Primary and Secondary ConnectionStrings to the NotificationHub
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}/AuthorizationRules/{authorizationRuleName}/listKeys
  tags: Notification Hubs Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulenamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulenamelistkeys-post-openapi.md
- name: Azure Notification Hubs API Notification Hubs Regenerate Keys
  x-api-slug: azure-notification-hubs-api
  description: Regenerates the Primary/Secondary Keys to the NotificationHub Authorization
    Rule
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.NotificationHubs/namespaces/{namespaceName}/notificationHubs/{notificationHubName}/AuthorizationRules/{authorizationRuleName}/regenerateKeys
  tags: Notification Hubs Regenerate Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-notificationhubsnamespacesnamespacenamenotificationhubsnotificationhubnameauthorizationrulesauthorizationrulenameregeneratekeys-post-openapi.md
- name: Azure Notification Hubs API
  x-api-slug: azure-notification-hubs-api
  description: Azure Notification Hubs provide an easy-to-use, multi-platform, scaled-out
    push engine. With a single cross-platform API call, you can easily send targeted
    and personalized push notifications to any mobile platform from any cloud or on-premises
    backend.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-notification-hubs.png
  humanURL: https://docs.microsoft.com/en-us/azure/notification-hubs/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-notification-hubs/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/rest/api/notificationhubs
- type: x-website
  url: https://docs.microsoft.com/en-us/azure/notification-hubs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---