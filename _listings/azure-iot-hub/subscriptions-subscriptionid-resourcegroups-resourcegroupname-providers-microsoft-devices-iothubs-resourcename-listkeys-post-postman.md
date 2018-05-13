{
  "info": {
    "name": "Azure IoT Hub API Iot Hub Resource List Keys",
    "_postman_id": "4e658eb3-bae9-45bf-9293-1639de6dc9c1",
    "description": "Get the security metadata for an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-security.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "iot hub resource keys",
      "item": [
        {
          "id": "46b4253b-271c-4b7b-838e-b1e39bdd3df5",
          "name": "IotHubResource_ListKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Devices/IotHubs/:resourceName/listkeys"
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceName",
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
            "description": "Get the security metadata for an IoT hub"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93c5c596-af3c-45cc-a850-fc63a306ea10"
            }
          ]
        }
      ]
    }
  ]
}