{
  "info": {
    "name": "Plentymarkets Get Export Key",
    "_postman_id": "7c8ef387-91d0-4d01-94b8-a6da367c1ea0",
    "description": "Get export keys..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Keys",
      "item": [
        {
          "id": "7c54d966-40f3-4490-9d52-7b051ced0fbd",
          "name": "getExportExportkey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "export/:exportKey"
              ],
              "variable": [
                {
                  "id": "exportKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get export keys."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cb55170-5ddc-439b-ad3f-f9ebf3ba4e29"
            }
          ]
        },
        {
          "id": "75b74fc0-8b01-4c8f-a5ee-d5c951d2762d",
          "name": "getExportExportkeyToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "export/:exportKey/:token"
              ],
              "variable": [
                {
                  "id": "exportKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get export keys.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c089c01-a077-4869-a388-d2ce37111090"
            }
          ]
        }
      ]
    }
  ]
}