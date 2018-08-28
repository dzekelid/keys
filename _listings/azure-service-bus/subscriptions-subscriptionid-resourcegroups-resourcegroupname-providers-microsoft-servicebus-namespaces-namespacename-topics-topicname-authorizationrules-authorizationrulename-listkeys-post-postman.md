{
  "info": {
    "name": "Azure Service Bus API Topics List Keys",
    "_postman_id": "6e560545-13a2-4824-9040-e6ff56ddd032",
    "description": "Gets the primary and secondary connection strings for the topic.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "topics keys",
      "item": [
        {
          "id": "495263bc-0fb2-46e8-9e0c-18d070805ab0",
          "name": "Topics_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ServiceBus/namespaces/:namespaceName/topics/:topicName/authorizationRules/:authorizationRuleName/ListKeys"
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
                  "id": "topicName",
                  "value": "topicName",
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
            "description": "Gets the primary and secondary connection strings for the topic"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3ed29ea-9162-4bc3-bf58-3b19ba69b518"
            }
          ]
        }
      ]
    }
  ]
}