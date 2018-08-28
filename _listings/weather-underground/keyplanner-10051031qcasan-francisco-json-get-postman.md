{
  "info": {
    "name": "Weather Underground Get Key Planner 10051031 Q Ca San Francisco",
    "_postman_id": "c61b9216-7549-4189-ba9f-bf701e61d9bb",
    "description": "This example will return a Historical roll up of weather data in San Francisco from Oct 5 to Oct 31. An example application: http://www.wunderground.com/travelplanner/index.asp",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Weather",
      "item": [
        {
          "id": "a32cc455-b748-445b-b6de-dcbc8c34573a",
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
              "id": "69066eca-8070-4749-b81c-f34a3bb52868"
            }
          ]
        },
        {
          "id": "48445fbf-359f-482e-ba09-3270a1d15a0d",
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
              "id": "3879b0b7-3ed2-410e-9827-2e900d565c39"
            }
          ]
        },
        {
          "id": "02946028-8706-4661-9152-559688036f67",
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
              "id": "6c824dd4-28c0-4c00-829d-3007b7e8a159"
            }
          ]
        },
        {
          "id": "c17bc336-cf8b-461f-b693-54135b02759c",
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
              "id": "8b04d160-373c-438f-b584-d9500b62ce7f"
            }
          ]
        },
        {
          "id": "75768cfb-f685-4c6d-b1e6-a1be7e05ecd4",
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
              "id": "e0d74724-3160-41b9-8ce4-b13dac4c7888"
            }
          ]
        },
        {
          "id": "742bedd3-0ed7-4e0c-ade1-5ccd4d7c5f8c",
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
              "id": "0128451b-86b1-4afa-9460-318d995b52c9"
            }
          ]
        },
        {
          "id": "a4badac8-2482-4cc7-945c-864e40726b96",
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
              "id": "f08d067a-e431-4f83-89e4-5f02e5431826"
            }
          ]
        },
        {
          "id": "72220d58-835b-4496-86ec-b3862566967a",
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
              "id": "b9fcc84c-8162-492d-9f3f-d4bc851a0eea"
            }
          ]
        },
        {
          "id": "7cd74159-3354-4256-9646-f39b1c3de45a",
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
              "id": "84afc06e-4090-4ca6-ac4a-7ad4b0a31a82"
            }
          ]
        },
        {
          "id": "129580f6-9c9d-4148-bb0a-9fb4009d7df8",
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
              "id": "027d223b-384e-4ba0-a6ef-87712c2372c7"
            }
          ]
        },
        {
          "id": "4ea07e21-7dd3-4d87-a2db-7d6f5862aac2",
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
              "id": "1eab1d71-2dd6-435c-a900-b405a9fa0faf"
            }
          ]
        },
        {
          "id": "213e0e51-33af-4a26-8260-438209726bc8",
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
              "id": "37ebba92-c6bb-480c-a09e-22beb1c6f02e"
            }
          ]
        },
        {
          "id": "56ce3c4d-d6c6-4e16-9304-6daf7ec88fd5",
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
              "id": "46e01b03-487c-4bca-b81e-256e407e485e"
            }
          ]
        },
        {
          "id": "19987089-659b-4998-8197-6a68a886e752",
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
              "id": "dc16e3e6-6884-426d-a3ac-316179dc4574"
            }
          ]
        },
        {
          "id": "0c3745a9-5129-4ba4-a92f-de396355faeb",
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
              "id": "9f8fc9f7-7064-4901-be00-2ae495265872"
            }
          ]
        },
        {
          "id": "5162f86a-f396-436f-9be2-3898b42de530",
          "name": "Get_satellite_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/satellite/q/CA/San_Francisco.json"
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
            "description": "This example will return URL's for satellite (visual and IR) images for San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "055f996a-7d6e-4374-b163-32e278fba4d6"
            }
          ]
        },
        {
          "id": "10acfbe3-b0a1-4316-af2f-8afa79a05f8f",
          "name": "Get_radar_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/radar/image.gif?maxlat=42.35%26maxlon=-109.311%26minlat=39.27%26minlon=-114.644%26width=600%26height=480%26newmaps=0"
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
            "description": "This example will return dynamic radar image around Salt Lake City, UT with a transparent background. See Docs for all the options for creating these images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c2dcbae-834e-4e7f-87bf-2d693d7d2904"
            }
          ]
        },
        {
          "id": "e3c91d92-5412-4b5c-9475-4904df4bb61d",
          "name": "Get_radar_example2_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/radar/image.gif?maxlat=42.35%26maxlon=-109.311%26minlat=39.27%26minlon=-114.644%26width=600%26height=480%26newmaps=1"
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
            "description": "This example will return dynamic radar image around Salt Lake City, UT with a Base Map background. See Docs for all the options for creating these images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06b71749-c89b-4059-a7d9-a9f7c317397c"
            }
          ]
        },
        {
          "id": "20cdb8a8-2d14-47e3-9a6e-42a104400dec",
          "name": "Get_alerts_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/alerts/q/CA/San_Francisco.json"
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
            "description": "This example will return active severe alerts for San Francisco, California.    This request only works in the USA, Canada and Europe."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a36abb24-d022-40a0-af6c-3644b6002ad9"
            }
          ]
        },
        {
          "id": "0184d9c9-9e43-4f3d-b8bc-0b501a894498",
          "name": "Get_Tide_example1_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/tide/q/CA/San_Francisco.json"
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
            "description": "This example will return 4 days of tides for San Francisco, California starting 'today'.    This request only works in the USA."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4a50b6a-b651-404e-9cab-7333f5c7c2aa"
            }
          ]
        },
        {
          "id": "900f3549-eb70-4b01-bdc7-1cd79f09a2f9",
          "name": "Get_Tide_example2_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/tide_20160312/q/CA/San_Francisco.json"
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
            "description": "This example will return 4 days of tides for San Francisco, California following March 3 2012.    This request only works in the USA."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "744d7e18-3a76-454f-9bdb-c045e44c0563"
            }
          ]
        },
        {
          "id": "17de2a0e-9f83-4c09-a43a-423b2c6c1bab",
          "name": "Get_Tide_RAW_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/rawtide_20160312/q/CA/San_Francisco.json"
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
            "description": "This example will return raw tide data for San Francisco, California on March 3 2016.    This request only works in the USA."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "449063e6-d621-4cfb-8d1b-1f526ee72efe"
            }
          ]
        },
        {
          "id": "9c6b3a10-2ac1-4879-815b-20384fab458c",
          "name": "Get_TenDay_hourly_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/hourly10day/q/CA/San_Francisco.json"
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
            "description": "This example will return a detailed hourly forecast for the next 10 days in San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06d4668a-0c3a-42e5-bef3-c3d844425057"
            }
          ]
        },
        {
          "id": "4f1f7aae-fa66-45a4-b136-53f6a8784d65",
          "name": "Get_yesterday_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/yesterday/q/CA/San_Francisco.json"
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
            "description": "This example will return yesterday's weather in San Francisco, California."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d65c075-b24e-4848-b17e-df529a8d1711"
            }
          ]
        },
        {
          "id": "9ba4b22d-40ef-4542-9d83-e24713309a44",
          "name": "Get_Planner_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/planner_10051031/q/CA/San_Francisco.json"
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
            "description": "This example will return a Historical roll up of weather data in San Francisco from Oct 5 to Oct 31. An example application: http://www.wunderground.com/travelplanner/index.asp"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c33bdb89-92f8-40d8-866f-7dd995523f73"
            }
          ]
        }
      ]
    }
  ]
}