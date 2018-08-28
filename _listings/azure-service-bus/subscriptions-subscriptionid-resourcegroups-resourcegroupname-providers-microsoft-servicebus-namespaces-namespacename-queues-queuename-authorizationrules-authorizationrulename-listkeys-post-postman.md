{
  "info": {
    "name": "Azure Service Bus API Queues List Keys",
    "_postman_id": "aa9ddefa-f509-42be-8ab8-9f949be913fd",
    "description": "Primary and secondary connection strings to the queue.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "queues keys",
      "item": [
        {
          "id": "dc5e204a-e7d2-45c9-ad06-a87db0b5b518",
          "name": "Queues_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ServiceBus/namespaces/:namespaceName/queues/:queueName/authorizationRules/:authorizationRuleName/ListKeys"
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
                  "id": "queueName",
                  "value": "queueName",
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
            "description": "Primary and secondary connection strings to the queue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6a637b3-a0fe-47fd-aeb3-2f926426c7df"
            }
          ]
        }
      ]
    }
  ]
}