{
  "info": {
    "name": "Weather Underground Get Key Hourly Q Ca San Francisco",
    "_postman_id": "082ab10d-02f1-4907-9959-4da780189973",
    "description": "This example will return a detailed hourly forecast for the 'next' 36 hours in San Francisco, California",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Weather",
      "item": [
        {
          "id": "f7f4edd7-30bf-46ce-a449-dbcac5e00d55",
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
              "id": "7e5f4b3e-d724-43b7-8ee1-5c29de693683"
            }
          ]
        },
        {
          "id": "eda29dc7-d6cc-4330-89b0-8aeaa820bdbe",
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
              "id": "0d6c0f09-21eb-40d3-bd4c-2585ca50fcc0"
            }
          ]
        },
        {
          "id": "33ca1081-765d-4fd3-9fb5-7be1338aba93",
          "name": "Get_IPAddress_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/autoip.json"
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
            "description": "This example will return the geographic attributes associated with the IP address location of the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a02b8fc3-b8a4-4e87-9c48-03dd6c1ad1d3"
            }
          ]
        },
        {
          "id": "0ba00418-a08a-49b3-8ed9-8a43b8b00636",
          "name": "Get_ZIP_geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/94107.json"
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
            "description": "This example will return the geographic attributes of zip code 94107"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5597ac7-2a49-4708-b26f-4ec2762b1027"
            }
          ]
        },
        {
          "id": "a6f6eff7-d03a-415e-a792-4ef1be3526b4",
          "name": "Get_Airport_geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/SFO.json"
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
            "description": "This example will return the geographic attributes of San Francisco International Airport (Airport Code: SFO)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14dedf0d-7db5-4fdc-a7ec-dba96c4b30cc"
            }
          ]
        },
        {
          "id": "f504eaa3-57a9-439c-b953-43a8ad6f47ae",
          "name": "Get_Lat_Long_geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/37.776289,-122.395234.json"
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
            "description": "This example will return the the geographic attributes of Latitude 37.776289 N, Longitude 122.395234 W"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce11b2c0-b6ee-4ba0-acae-b836521d53b6"
            }
          ]
        },
        {
          "id": "5b4818b7-cb1a-4bfd-9431-88b8882f1376",
          "name": "Get_pws_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/q/pws:KCATAHOE2.json"
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
            "description": "This example will return the the current weather conditions at the Personal Weather Station (pws) KCATAHOE2"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0352d503-edcc-42bc-b049-2c531d52b4fe"
            }
          ]
        },
        {
          "id": "3d6df09f-1a82-49aa-96fc-280e51ca5a92",
          "name": "Get_Conditions_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/q/CA/San_Francisco.json"
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
            "description": "This example will return the current conditions in San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7164bd2-c70d-47f9-ba9e-042a23a8aa30"
            }
          ]
        },
        {
          "id": "71267f79-0f65-4584-b72b-bb66670cee92",
          "name": "Get_Astronomy_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/astronomy/q/CA/San_Francisco.json"
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
            "description": "This example will return the Astronomy of San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9c8cf5e-3ab4-4c8e-8438-194524933bea"
            }
          ]
        },
        {
          "id": "d794fd9d-7f41-4bdc-a225-befce865d310",
          "name": "Get_forecast3_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/forecast/q/CA/San_Francisco.json"
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
            "description": "This example will return the 3 Day Forecast Summary for San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58648065-2e8e-4827-9e4b-cc0d870559e2"
            }
          ]
        },
        {
          "id": "6effe5c1-3f7e-405e-afec-e1e80bd7efb9",
          "name": "Get_almanac_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/almanac/q/CA/San_Francisco.json"
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
            "description": "This example will return Today's Average Highs/Lows and Record Highs/Lows for San Francisco, California."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a230a87-fbe6-4cdf-b1bd-b414278fc2a7"
            }
          ]
        },
        {
          "id": "c2fc8ce9-7f29-4a5e-bbcc-4fa4f4a25167",
          "name": "Get_French_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/forecast/lang:FR/q/France/Paris.json"
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
            "description": "This example will return Current Conditions and a 3 day simple Forecast for Paris France in French. See documentation page for full list of language code options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ee6bf0f-dbcc-474b-a786-1cfd86264dde"
            }
          ]
        },
        {
          "id": "a31e4c2e-b75e-4035-9c20-28ea0d269f08",
          "name": "Get_Spanish_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/forecast/lang:SP/q/Spain/Alicante.json"
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
            "description": "This example will return Current Conditions and a 3 day simple Forecast for Alicante, Spain in Spanish. See documentation page for full list of language code options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94f9fb78-6a0b-4d25-af32-e251651825e0"
            }
          ]
        },
        {
          "id": "ccd12d4e-a0e8-4a15-af44-ebb5abb201d6",
          "name": "Get_forecast10_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/forecast10day/q/CA/San_Francisco.json"
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
            "description": "This example will return the 10 Day Forecast Summary for San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d34f1e7e-f333-483a-988d-44b544bfb520"
            }
          ]
        },
        {
          "id": "0ae24ebc-02ca-4678-a5fd-508315212747",
          "name": "Get_OneDay_hourly_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/hourly/q/CA/San_Francisco.json"
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
            "description": "This example will return a detailed hourly forecast for the 'next' 36 hours in San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "201845fe-1d22-435e-b5ca-843e0ad85ca3"
            }
          ]
        }
      ]
    }
  ]
}