{
  "info": {
    "name": "Weather Underground Get Key Geolookup Q France Paris",
    "_postman_id": "4dd1c729-e3f5-44de-acf4-c1f3995075e5",
    "description": "This example will return the geographic attributes of Paris, France. Use {Full Country Name} / {City Name}",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Weather",
      "item": [
        {
          "id": "ee1a983a-37c4-4353-b7f6-bd5af7b6e49a",
          "name": "Get_USA_Geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/CA/San_Francisco.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the geographic attributes of San Francisco CA.    Use {2 letter state code} /    {City Name}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "940c3be1-9c6b-4b3d-b850-7be6e2139038"
            }
          ]
        },
        {
          "id": "469c8392-915d-4b21-93c1-e1b6ad48b23e",
          "name": "Get_Outside_of_USA_Geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/France/Paris.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the geographic attributes of Paris, France. Use {Full Country Name} / {City Name}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ac4edb8-aa1a-45de-a620-6d360468fde3"
            }
          ]
        }
      ]
    }
  ]
}