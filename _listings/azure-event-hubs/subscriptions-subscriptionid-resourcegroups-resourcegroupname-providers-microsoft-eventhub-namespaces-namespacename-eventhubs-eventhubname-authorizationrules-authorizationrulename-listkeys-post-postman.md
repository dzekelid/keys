{
  "info": {
    "name": "Azure Event Hubs API Event Hubs List Keys",
    "_postman_id": "d88b4ed4-39da-40ae-a081-6be8baf14223",
    "description": "Gets the ACS and SAS connection strings for the Event Hub.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "event hubs keys",
      "item": [
        {
          "id": "9eb9a46e-a2eb-4796-b5f6-a376edcd6b17",
          "name": "EventHubs_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.EventHub/namespaces/:namespaceName/eventhubs/:eventHubName/authorizationRules/:authorizationRuleName/ListKeys"
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
                  "id": "eventHubName",
                  "value": "eventHubName",
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
            "description": "Gets the ACS and SAS connection strings for the Event Hub"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e39deb3-54cf-44d1-b8de-bafc9d455dc1"
            }
          ]
        }
      ]
    }
  ]
}