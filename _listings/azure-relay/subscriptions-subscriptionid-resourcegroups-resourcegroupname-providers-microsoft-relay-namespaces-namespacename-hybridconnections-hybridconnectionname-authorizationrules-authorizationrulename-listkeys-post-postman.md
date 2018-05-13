{
  "info": {
    "name": "Azure Relay API Hybrid Connections List Keys",
    "_postman_id": "13ecc810-5bbc-41db-bf64-98615b580570",
    "description": "Primary and Secondary ConnectionStrings to the HybridConnection.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hybrid connections keys",
      "item": [
        {
          "id": "f5343577-4bfb-4811-a4b3-bcc89dcde66f",
          "name": "HybridConnections_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/HybridConnections/:hybridConnectionName/authorizationRules/:authorizationRuleName/ListKeys"
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
                  "id": "hybridConnectionName",
                  "value": "hybridConnectionName",
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
            "description": "Primary and Secondary ConnectionStrings to the HybridConnection"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "473d4a19-3e62-419c-bbcf-6f0a592ae9d5"
            }
          ]
        }
      ]
    }
  ]
}