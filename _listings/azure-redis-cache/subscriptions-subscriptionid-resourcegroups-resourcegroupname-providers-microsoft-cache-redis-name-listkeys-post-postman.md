{
  "info": {
    "name": "Azure Redis Cache API Redis List Keys",
    "_postman_id": "64f5cd8a-8769-475e-9dec-fd07e9df3ea3",
    "description": "Retrieve a Redis cache's access keys. This operation requires write permission to the cache resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "redis keys",
      "item": [
        {
          "id": "73952862-3a37-4807-abc5-e72f2a4ca511",
          "name": "Redis_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Cache/Redis/:name/listKeys"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a Redis cache's access keys"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8ecc699-f908-4437-a5c7-e8742f9aefff"
            }
          ]
        }
      ]
    }
  ]
}