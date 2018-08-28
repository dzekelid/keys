{
  "info": {
    "name": "Launch Darkly Modify a project by ID",
    "_postman_id": "82437332-ca48-475f-b65f-d25739175b99",
    "description": "Modify a project by id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "e0683e22-4165-444b-8a02-8d1761751e85",
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
              "id": "873f8b1c-03fc-4edc-aec1-bdd178376f0b"
            }
          ]
        },
        {
          "id": "ae66edce-fa24-43dc-8e7d-d8e0639a05f6",
          "name": "getEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey/:environmentKey"
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
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get an environment by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59abea20-3dd8-4c5c-bbba-5a76aa41d947"
            }
          ]
        },
        {
          "id": "5fb62dca-a3c4-48ae-8442-81a11e62388e",
          "name": "deleteEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey/:environmentKey"
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
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an environment by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61192155-19da-484c-8e4e-6585fba13c5c"
            }
          ]
        },
        {
          "id": "748c9f2b-675f-4235-ab22-8d6fd22ae025",
          "name": "patchEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey/:environmentKey"
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
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Modify an environment by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d1b51a1-96a9-4b53-b038-28654cdf8e03"
            }
          ]
        }
      ]
    },
    {
      "name": "Flag-statuses",
      "item": [
        {
          "id": "47e62625-b701-428a-8936-b52018de1fb9",
          "name": "getFeatureFlagStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flag-statuses/:projectKey/:environmentKey"
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
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of statuses for all feature flags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23777c7d-4e84-4c90-8e47-2addcce4acc9"
            }
          ]
        },
        {
          "id": "579b54f4-30fb-4cd0-8c54-ef13a34155bd",
          "name": "getFeatureFlagStatuses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flag-statuses/:projectKey/:environmentKey/:featureFlagKey"
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
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of statuses for all feature flags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a0139e8-c7e5-459e-b929-e7f20855fefb"
            }
          ]
        }
      ]
    },
    {
      "name": "Flags",
      "item": [
        {
          "id": "efb710d5-c117-465e-8d4c-c1ba0a4ad5ed",
          "name": "getFeatureFlags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all features in the given project.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97db6609-3d16-463d-9858-5b2ac0bd6409"
            }
          ]
        },
        {
          "id": "7e21b631-22ce-453d-b4e4-485d47e1a248",
          "name": "postFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey"
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
            "description": "Create a feature flag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "954f25ea-763b-4dbf-b7fe-6de8dc08b331"
            }
          ]
        },
        {
          "id": "8ff94bb1-4244-4aed-9645-af6cc4da2542",
          "name": "getFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey/:featureFlagKey"
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
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single feature flag by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "018de390-144c-4772-bc08-a21e85644081"
            }
          ]
        },
        {
          "id": "3a11d7ba-510d-440e-8f55-c26f2179f69c",
          "name": "deleteFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey/:featureFlagKey"
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
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a feature flag by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b545dbdc-9947-4526-838f-d8f3b5bae525"
            }
          ]
        },
        {
          "id": "e69f70a4-5972-4239-a1a6-80b81ac36164",
          "name": "patchFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey/:featureFlagKey"
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
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a feature flag by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "296bb3da-09a5-4f7e-8131-1220b36be979"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "811e5db0-469e-4e21-bf1e-b79ad6680bb9",
          "name": "getProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "projects/:projectKey"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a project by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1b127a4-9e93-4372-a84e-704a8e6cb293"
            }
          ]
        },
        {
          "id": "c29d2024-cd17-4d3d-a1d0-787f3f3f74c4",
          "name": "deleteProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "projects/:projectKey"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a project by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3525816e-33f6-49f4-b3a9-726630fd5a3e"
            }
          ]
        },
        {
          "id": "2f0c2e7c-1310-4c94-958b-4868918fec93",
          "name": "patchProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "projects/:projectKey"
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
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a project by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99918e55-9b1a-4b74-8f13-f82703a5d588"
            }
          ]
        }
      ]
    }
  ]
}