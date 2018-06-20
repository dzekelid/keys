---
swagger: "2.0"
x-collection-name: Azure Event Hubs
x-complete: 1
info:
  title: EventHubManagementClient
  description: azure-event-hubs-client
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/listKeys
  : post:
      summary: Namespaces List Keys
      description: Gets the primary and secondary connection strings for the Namespace.
      operationId: Namespaces_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameauthorizationrulesauthorizationrulenamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Namespaces Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/regenerateKeys
  : post:
      summary: Namespaces Regenerate Keys
      description: Regenerates the primary or secondary connection strings for the
        specified Namespace.
      operationId: Namespaces_RegenerateKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameauthorizationrulesauthorizationrulenameregeneratekeys-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters required to regenerate the connection string
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Namespaces Regenerate Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/eventhubs/{eventHubName}/authorizationRules/{authorizationRuleName}/ListKeys
  : post:
      summary: Event Hubs List Keys
      description: Gets the ACS and SAS connection strings for the Event Hub.
      operationId: EventHubs_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameauthorizationrulesauthorizationrulenamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Event Hubs Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/eventhubs/{eventHubName}/authorizationRules/{authorizationRuleName}/regenerateKeys
  : post:
      summary: Event Hubs Regenerate Keys
      description: Regenerates the ACS and SAS connection strings for the Event Hub.
      operationId: EventHubs_RegenerateKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameauthorizationrulesauthorizationrulenameregeneratekeys-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to regenerate the AuthorizationRule Keys
          (PrimaryKey/SecondaryKey)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Event Hubs Regenerate Keys
---