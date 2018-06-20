{
  "info": {
    "name": "Launch Darkly Create an environment",
    "_postman_id": "4acb18b4-d312-4a0c-81d1-b9b9eae499ef",
    "description": "Create an environment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "5204fe9e-7377-4835-a60f-7e8bd9209609",
          "name": "postEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey"
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
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "610a13ba-d5ae-4618-ae7a-3a93c8c5360c"
            }
          ]
        }
      ]
    }
  ]
}