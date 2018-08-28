{
  "info": {
    "name": "Azure Media Services API Media Service List Keys",
    "_postman_id": "2e6c15dc-f91c-4564-8430-beae0e6a07bb",
    "description": "Lists the keys for a Media Service.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "media service keys",
      "item": [
        {
          "id": "983bfca5-7908-42e9-a7af-64c7141bb520",
          "name": "MediaService_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Media/mediaservices/:mediaServiceName/listKeys"
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
                  "id": "mediaServiceName",
                  "value": "mediaServiceName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the keys for a Media Service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c6a1aee-cca8-4c5b-969c-854ce9ec58b6"
            }
          ]
        }
      ]
    }
  ]
}