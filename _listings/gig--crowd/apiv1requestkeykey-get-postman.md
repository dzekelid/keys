{
  "info": {
    "name": "GIGANDCROWD Get Request Key Key",
    "_postman_id": "64b149da-eb49-4025-bc2d-e51530de7e56",
    "description": "Get request key key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "2a85e43b-fdc6-4b52-b7bd-5ecec44b1001",
          "name": "getApiV1RequestKeyKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/key/:key"
              ],
              "variable": [
                {
                  "id": "key",
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
            "description": "Get request key key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0811477-00fa-416c-8f23-615a063b6d65"
            }
          ]
        }
      ]
    }
  ]
}