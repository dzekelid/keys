{
  "info": {
    "name": "Azure Machine Learning API Web Services List Keys",
    "_postman_id": "fd63f9e8-92a2-4914-97a1-db426d56415f",
    "description": "Gets the access keys for the specified web service.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "web services keys",
      "item": [
        {
          "id": "19ed82d2-80c7-4ca3-a2ca-84a0adab9b2c",
          "name": "WebServices_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.MachineLearning/webServices/:webServiceName/listKeys"
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
                  "id": "webServiceName",
                  "value": "webServiceName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the access keys for the specified web service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3b1be29-7b2c-47d8-bd35-f9b49cb7dffa"
            }
          ]
        }
      ]
    }
  ]
}