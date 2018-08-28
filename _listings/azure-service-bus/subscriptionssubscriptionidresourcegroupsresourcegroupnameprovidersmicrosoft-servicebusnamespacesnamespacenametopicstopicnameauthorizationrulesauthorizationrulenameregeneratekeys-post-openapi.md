---
swagger: "2.0"
x-collection-name: Azure Service Bus
x-complete: 0
info:
  title: Azure Service Bus API Topics Regenerate Keys
  description: Regenerates primary or secondary connection strings for the topic.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ServiceBus/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/listKeys
  : post:
      summary: Namespaces List Keys
      description: Gets the primary and secondary connection strings for the namespace.
      operationId: Namespaces_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-servicebusnamespacesnamespacenameauthorizationrulesauthorizationrulenamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Namespaces Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ServiceBus/namespaces/{namespaceName}/AuthorizationRules/{authorizationRuleName}/regenerateKeys
  : post:
      summary: Namespaces Regenerate Keys
      description: Regenerates the primary or secondary connection strings for the
        namespace.
      operationId: Namespaces_RegenerateKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-servicebusnamespacesnamespacenameauthorizationrulesauthorizationrulenameregeneratekeys-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to regenerate the authorization rule
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Namespaces Regenerate Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ServiceBus/namespaces/{namespaceName}/queues/{queueName}/authorizationRules/{authorizationRuleName}/ListKeys
  : post:
      summary: Queues List Keys
      description: Primary and secondary connection strings to the queue.
      operationId: Queues_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-servicebusnamespacesnamespacenamequeuesqueuenameauthorizationrulesauthorizationrulenamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Queues Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ServiceBus/namespaces/{namespaceName}/queues/{queueName}/authorizationRules/{authorizationRuleName}/regenerateKeys
  : post:
      summary: Queues Regenerate Keys
      description: Regenerates the primary or secondary connection strings to the
        queue.
      operationId: Queues_RegenerateKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-servicebusnamespacesnamespacenamequeuesqueuenameauthorizationrulesauthorizationrulenameregeneratekeys-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to regenerate the authorization rule
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Queues Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ServiceBus/namespaces/{namespaceName}/topics/{topicName}/authorizationRules/{authorizationRuleName}/ListKeys
  : post:
      summary: Topics List Keys
      description: Gets the primary and secondary connection strings for the topic.
      operationId: Topics_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-servicebusnamespacesnamespacenametopicstopicnameauthorizationrulesauthorizationrulenamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Topics Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ServiceBus/namespaces/{namespaceName}/topics/{topicName}/authorizationRules/{authorizationRuleName}/regenerateKeys
  : post:
      summary: Topics Regenerate Keys
      description: Regenerates primary or secondary connection strings for the topic.
      operationId: Topics_RegenerateKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-servicebusnamespacesnamespacenametopicstopicnameauthorizationrulesauthorizationrulenameregeneratekeys-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to regenerate the authorization rule
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Topics Keys
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