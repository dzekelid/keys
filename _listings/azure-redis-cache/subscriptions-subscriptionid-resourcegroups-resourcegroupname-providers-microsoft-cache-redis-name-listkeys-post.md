---
swagger: "2.0"
info:
  title: RedisManagementClient
  description: REST API for Azure Redis Cache Service.
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
      description: Retrieve a Redis cache's access keys
      operationId: Redis_ListKeys
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
      - redis keys
definitions:
  Sku:
    properties:
      name:
        description: This is a default description.
        type: get
      family:
        description: This is a default description.
        type: get
      capacity:
        description: This is a default description.
        type: get
  RedisProperties:
    properties:
      redisConfiguration:
        description: This is a default description.
        type: get
      enableNonSslPort:
        description: This is a default description.
        type: get
      tenantSettings:
        description: This is a default description.
        type: get
      shardCount:
        description: This is a default description.
        type: get
      subnetId:
        description: This is a default description.
        type: get
      staticIP:
        description: This is a default description.
        type: get
  RedisCreateProperties:
    properties: []
  RedisUpdateProperties:
    properties:
      tags:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  RedisCreateParameters:
    properties: []
  RedisUpdateParameters:
    properties: []
  RedisAccessKeys:
    properties:
      primaryKey:
        description: This is a default description.
        type: get
      secondaryKey:
        description: This is a default description.
        type: get
  RedisFirewallRule:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  RedisFirewallRuleProperties:
    properties:
      startIP:
        description: This is a default description.
        type: get
      endIP:
        description: This is a default description.
        type: get
  RedisFirewallRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  RedisResourceProperties:
    properties:
      redisVersion:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      hostName:
        description: This is a default description.
        type: get
      port:
        description: This is a default description.
        type: get
      sslPort:
        description: This is a default description.
        type: get
  RedisResource:
    properties: []
  RedisListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  RedisRegenerateKeyParameters:
    properties:
      keyType:
        description: This is a default description.
        type: get
  RedisRebootParameters:
    properties:
      rebootType:
        description: This is a default description.
        type: get
      shardId:
        description: This is a default description.
        type: get
  ExportRDBParameters:
    properties:
      format:
        description: This is a default description.
        type: get
      prefix:
        description: This is a default description.
        type: get
      container:
        description: This is a default description.
        type: get
  ImportRDBParameters:
    properties:
      format:
        description: This is a default description.
        type: get
      files:
        description: This is a default description.
        type: get
  ScheduleEntry:
    properties:
      dayOfWeek:
        description: This is a default description.
        type: get
      startHourUtc:
        description: This is a default description.
        type: get
      maintenanceWindow:
        description: This is a default description.
        type: get
  ScheduleEntries:
    properties:
      scheduleEntries:
        description: This is a default description.
        type: get
  RedisPatchSchedule:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
  RedisForceRebootResponse:
    properties:
      Message:
        description: This is a default description.
        type: get
  Operation:
    properties:
      name:
        description: This is a default description.
        type: get
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
x-collection-name: Azure Redis Cache
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