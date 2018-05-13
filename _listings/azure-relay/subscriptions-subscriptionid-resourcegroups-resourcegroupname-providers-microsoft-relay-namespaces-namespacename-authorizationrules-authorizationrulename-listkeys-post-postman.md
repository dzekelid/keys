{
  "info": {
    "name": "Azure Relay API Namespaces List Keys",
    "_postman_id": "0b9f26f1-0aa4-47a6-8ffb-ba7b8da9b2fb",
    "description": "Primary and Secondary ConnectionStrings to the namespace",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "namespaces keys",
      "item": [
        {
          "id": "c925cd33-034f-4b2d-8c47-c63fe0ac2671",
          "name": "Namespaces_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/AuthorizationRules/:authorizationRuleName/listKeys"
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
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "namespaceName",
                  "value": "namespaceName",
                  "type": "string"
                },
                {
                  "id": "authorizationRuleName",
                  "value": "authorizationRuleName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Primary and Secondary ConnectionStrings to the namespace "
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fdfe38a-c291-4dcf-a13c-72f82c19039f"
            }
          ]
        }
      ]
    }
  ]
}