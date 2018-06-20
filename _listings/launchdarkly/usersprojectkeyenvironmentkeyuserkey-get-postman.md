{
  "info": {
    "name": "Launch Darkly Get a user by key.",
    "_postman_id": "237807ba-7271-4f58-8a53-8610b8772eea",
    "description": "Get a user by key..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "a3fdeb45-3f2c-49a0-bb2e-ac08ad845a20",
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
              "id": "b71e83b1-18ec-4a39-b22d-2c44ebd9e270"
            }
          ]
        },
        {
          "id": "8c533c32-6872-45f0-aec9-4abce81722fa",
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
              "id": "c6c4901c-394e-4c87-add5-6e1aa96aee18"
            }
          ]
        },
        {
          "id": "037f980c-4efd-4003-af00-5bbd817c6d81",
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
              "id": "b504d8ce-5080-4112-9ce6-72598684b2a8"
            }
          ]
        },
        {
          "id": "87d8771f-a3c4-4053-84b7-f41c68cce36f",
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
              "id": "9ef42cc7-e9d1-4d1d-b2a4-36b3b5fda283"
            }
          ]
        }
      ]
    },
    {
      "name": "Flag-statuses",
      "item": [
        {
          "id": "7b0d3cc0-6871-4314-86f4-057c5dd9b3b9",
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
              "id": "10a110cd-58ad-4876-9b54-8df563d642f3"
            }
          ]
        },
        {
          "id": "b902e66b-0bc1-4e0a-8a81-bebcade64098",
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
              "id": "aabe69c5-cbed-4b94-873a-e7463bfc473c"
            }
          ]
        }
      ]
    },
    {
      "name": "Flags",
      "item": [
        {
          "id": "0505c9eb-c700-4e46-8162-15e7877e020d",
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
              "id": "b3b6c3b1-0301-4f7c-97e8-480df4000506"
            }
          ]
        },
        {
          "id": "e30b52cf-9195-426f-8214-e6de015035b5",
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
              "id": "8549089b-4ec7-40e7-a8f9-db9373324074"
            }
          ]
        },
        {
          "id": "ed7426c3-9977-45d6-9912-161d1d2e90b5",
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
              "id": "5ea5214e-e4b1-41be-9e15-2c167e96824f"
            }
          ]
        },
        {
          "id": "4f02b885-7b1f-452f-9544-39a5e8835171",
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
              "id": "213b04c0-44bf-4f23-a794-d5c8d522112e"
            }
          ]
        },
        {
          "id": "eded7cc4-6856-4594-83f7-1c32f8026986",
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
              "id": "50f2539b-2f0e-4d4b-93cb-d5a1cac3b008"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "1846b0c7-fc2c-4955-b4bd-fcca3c475c52",
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
              "id": "7e7d505d-d485-4801-ae99-54079871d54f"
            }
          ]
        },
        {
          "id": "bbc1d345-4029-473c-985c-402acbd5f04f",
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
              "id": "efe8551e-0783-4f56-8421-cc68802222b0"
            }
          ]
        },
        {
          "id": "3ace5496-08ed-4f04-a80c-255fac00b763",
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
              "id": "c7a609f5-96ac-424f-a5d6-e9ea130eb01e"
            }
          ]
        }
      ]
    },
    {
      "name": "User-search",
      "item": [
        {
          "id": "75ccfa2e-1bf1-4a4f-9760-32d29504e1ee",
          "name": "getSearchUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "user-search/:projectKey/:environmentKey"
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
            "description": "Search users in launchdarkly based on their last active date, or a search query.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c05b723b-fe9d-4e84-a6e7-5d4aab3301d5"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "8a79f8bc-4189-412c-bdde-49b895048e44",
          "name": "getUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey"
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
            "description": "List all users in the environment.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2708737b-9310-4d99-9da8-94e3b58e6d3e"
            }
          ]
        },
        {
          "id": "72046f54-785d-4033-b159-b4115c7d60f0",
          "name": "getUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey/:userKey"
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
                  "id": "userKey",
                  "value": "userKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e04362f0-4695-4328-b2e6-24eb8d02cca9"
            }
          ]
        },
        {
          "id": "a1136f85-4e34-4104-b97f-9ebe1fd99537",
          "name": "deleteUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey/:userKey"
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
                  "id": "userKey",
                  "value": "userKey",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a user by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6efc3a71-fe0c-4600-ad86-af8f6dfd84c8"
            }
          ]
        }
      ]
    }
  ]
}