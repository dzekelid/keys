{
  "info": {
    "name": "Weather Underground Get Key Geolookup Q Ca San Francisco",
    "_postman_id": "b745342d-24be-45a4-9b51-caf8260c349d",
    "description": "This example will return the geographic attributes of San Francisco CA.    Use {2 letter state code} /    {City Name}",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Weather",
      "item": [
        {
          "id": "f0adf5e8-aa17-41c6-9b76-3fd23e25aa27",
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
              "id": "16a2a137-49d7-4d11-b3dc-9804a672b95b"
            }
          ]
        }
      ]
    }
  ]
}