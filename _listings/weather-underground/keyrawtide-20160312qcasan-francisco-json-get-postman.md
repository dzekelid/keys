{
  "info": {
    "name": "Weather Underground Get Key Rawte 20160312 Q Ca San Francisco",
    "_postman_id": "97a9e09d-4b2c-4b64-9356-7f3bb5cd0072",
    "description": "This example will return raw tide data for San Francisco, California on March 3 2016.    This request only works in the USA.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Weather",
      "item": [
        {
          "id": "80b2313e-9e07-4d23-9224-54f80aa800dd",
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
              "id": "c39ca956-ab9b-476c-bbb9-9a7d3c488d58"
            }
          ]
        },
        {
          "id": "80799882-f261-4f98-bd0c-18b081ca5e18",
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
              "id": "3a92f776-a580-4ca1-984e-c466a2fc839f"
            }
          ]
        },
        {
          "id": "26e3d85b-682a-474b-9e9d-098899910030",
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
              "id": "4286b988-f494-4af1-a6cf-86c921f2c266"
            }
          ]
        },
        {
          "id": "0b2fcc5d-430a-4316-b490-e7e393455852",
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
              "id": "dfecd518-418e-4766-afc4-466eae60e78b"
            }
          ]
        },
        {
          "id": "5e1e1a23-6568-4dc8-bd70-4c3b10326b82",
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
              "id": "6aa6a415-a355-4c4a-a7a9-b68a08094c2f"
            }
          ]
        },
        {
          "id": "eff27aff-4925-4ff0-9aeb-6f283f853eff",
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
              "id": "71c0c029-fc07-40ad-828a-284072776189"
            }
          ]
        },
        {
          "id": "a18f4211-5179-4ece-8aff-d6e01e08ca23",
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
              "id": "3736e9ef-f3a3-4ca7-a6b0-458983463a03"
            }
          ]
        },
        {
          "id": "908b978a-a051-41cd-9815-3a8f4fbce764",
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
              "id": "055ae971-bfb3-47fe-a733-2685b703db57"
            }
          ]
        },
        {
          "id": "eae7a7ca-7bd0-43a0-8efa-d023e1e97740",
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
              "id": "128986a7-8672-402d-bb2a-034929f900af"
            }
          ]
        },
        {
          "id": "bab6ab7e-fe68-4b84-9049-888199b94d78",
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
              "id": "cb13322c-1716-464f-8a65-8f658ae63fee"
            }
          ]
        },
        {
          "id": "fd31e47c-e2ba-4d6f-8ad9-40be553140ac",
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
              "id": "6e4e826c-f986-45cd-a319-c71520a914b4"
            }
          ]
        },
        {
          "id": "bfc52c49-c759-42e1-afaf-2e24f0ef714c",
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
              "id": "1f8cb4d5-ae78-4f6d-9a30-61f10965a83c"
            }
          ]
        },
        {
          "id": "30f91d57-7f15-422d-af30-4bbe8c58374b",
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
              "id": "344e57ce-e935-4e88-a24e-24fca6b718d0"
            }
          ]
        },
        {
          "id": "72da7a90-a343-47e6-a502-39e628e33f0d",
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
              "id": "c35f4a1a-e50c-428a-9c6e-22ce59742041"
            }
          ]
        },
        {
          "id": "619d680e-59b6-4a43-a0b6-e49309506cb0",
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
              "id": "9d0e2a64-3a29-412f-a896-3d4f4fefd898"
            }
          ]
        },
        {
          "id": "f9c9c3a4-1610-4d35-89c0-8110b80dced0",
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
              "id": "a55bbc17-91cd-403e-b3c7-b12bb5d20dd4"
            }
          ]
        },
        {
          "id": "16478e3d-db11-4354-8d22-f25dcdf4d09c",
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
              "id": "614025a8-8824-461e-ad12-50b82d17c11b"
            }
          ]
        },
        {
          "id": "7ef30054-c0dc-4c78-a0f3-b7b973e80cc6",
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
              "id": "af190481-dd14-437b-950f-bf8324ebf9da"
            }
          ]
        },
        {
          "id": "ce826e26-9f20-4b49-8f55-b73b39088293",
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
              "id": "9c0b5e1c-4594-4586-9c95-de3ab126ad37"
            }
          ]
        },
        {
          "id": "c47ebbaa-78cd-44cc-9355-b3b821f40e0b",
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
              "id": "295fabd0-e861-4a26-a59a-37e051a44051"
            }
          ]
        },
        {
          "id": "1a97d622-da76-4332-91c1-d10139e93e00",
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
              "id": "e5577a8d-f7b9-4bff-8956-8e20452350b4"
            }
          ]
        },
        {
          "id": "5f9bf118-27f4-4d88-9ccb-68b8e6361950",
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
              "id": "ee8a387a-c1af-48d8-ac58-f2d6fb7e20c0"
            }
          ]
        }
      ]
    }
  ]
}