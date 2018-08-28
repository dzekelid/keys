---
name: Azure Event Hubs
x-slug: azure-event-hubs
description: Azure Event Hubs is a hyper-scale telemetry ingestion service that collects,
  transforms, and stores millions of events. As a distributed streaming platform,
  it gives you low latency and configurable time retention, which enables you to ingress
  massive amounts of telemetry into the cloud and read the data from multiple applications
  using publish-subscribe semantics.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Event Hubs API Namespaces List Keys
  x-api-slug: azure-event-hubs-api
  description: Gets the primary and secondary connection strings for the Namespace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/listKeys
  tags: Namespaces Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameauthorizationrulesauthorizationrulenamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameauthorizationrulesauthorizationrulenamelistkeys-post-openapi.md
- name: Azure Event Hubs API Namespaces Regenerate Keys
  x-api-slug: azure-event-hubs-api
  description: Regenerates the primary or secondary connection strings for the specified
    Namespace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/regenerateKeys
  tags: Namespaces Regenerate Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameauthorizationrulesauthorizationrulenameregeneratekeys-post-openapi.md
- name: Azure Event Hubs API Event Hubs List Keys
  x-api-slug: azure-event-hubs-api
  description: Gets the ACS and SAS connection strings for the Event Hub.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/eventhubs/{eventHubName}/authorizationRules/{authorizationRuleName}/ListKeys
  tags: Event Hubs Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameauthorizationrulesauthorizationrulenamelistkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameauthorizationrulesauthorizationrulenamelistkeys-post-openapi.md
- name: Azure Event Hubs API Event Hubs Regenerate Keys
  x-api-slug: azure-event-hubs-api
  description: Regenerates the ACS and SAS connection strings for the Event Hub.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/eventhubs/{eventHubName}/authorizationRules/{authorizationRuleName}/regenerateKeys
  tags: Event Hubs Regenerate Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameauthorizationrulesauthorizationrulenameregeneratekeys-post-openapi.md
- name: Azure Event Hubs API
  x-api-slug: azure-event-hubs-api
  description: Azure Event Hubs is a hyper-scale telemetry ingestion service that
    collects, transforms, and stores millions of events. As a distributed streaming
    platform, it gives you low latency and configurable time retention, which enables
    you to ingress massive amounts of telemetry into the cloud and read the data from
    multiple applications using publish-subscribe semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-event-hubs-stream.png
  humanURL: https://azure.microsoft.com/en-us/services/event-hubs/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-event-hubs/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/event-hubs/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/event-hubs/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/event-hubs/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/event-hubs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---