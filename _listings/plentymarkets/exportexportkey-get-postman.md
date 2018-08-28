{
  "info": {
    "name": "Plentymarkets Get Export Keys",
    "_postman_id": "0b929d9b-e25e-4b01-b9bf-2c88bb0cf8d4",
    "description": "Get export keys.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Keys",
      "item": [
        {
          "id": "0a4300a4-31f4-4b1f-a381-569f582e20c3",
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
              "id": "12564e54-6ed3-4c1e-b91b-ee3689be5241"
            }
          ]
        }
      ]
    }
  ]
}