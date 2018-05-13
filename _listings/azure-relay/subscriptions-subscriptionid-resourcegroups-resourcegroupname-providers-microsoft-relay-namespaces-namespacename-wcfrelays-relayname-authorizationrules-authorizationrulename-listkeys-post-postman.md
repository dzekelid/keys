{
  "info": {
    "name": "Azure Relay API WCFRelays List Keys",
    "_postman_id": "c49bedfb-5ef4-41f5-8662-d92d63262d64",
    "description": "Primary and Secondary ConnectionStrings to the WCFRelays.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "wcfrelays keys",
      "item": [
        {
          "id": "728ffbeb-19ec-4c92-b1ee-b2aaca418560",
          "name": "WCFRelays_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/WcfRelays/:relayName/authorizationRules/:authorizationRuleName/ListKeys"
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
                  "id": "relayName",
                  "value": "relayName",
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
            "description": "Primary and Secondary ConnectionStrings to the WCFRelays"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35e69d21-483b-4437-a38f-45805af8d4e9"
            }
          ]
        }
      ]
    }
  ]
}