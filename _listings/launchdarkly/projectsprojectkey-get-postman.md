{
  "info": {
    "name": "Launch Darkly Get a project by key.",
    "_postman_id": "322242cf-80cd-4dea-8ecb-55fd43dc4916",
    "description": "Get a project by key..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "fa02b481-ceb0-4463-b093-c9c053be9936",
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
              "id": "a1f7e2e9-89fc-4edc-9782-b1d797f3a71a"
            }
          ]
        },
        {
          "id": "8af90d1b-4b70-408f-a039-72f0c687ff49",
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
              "id": "9609d452-2824-4d6a-b083-bffb46db01bd"
            }
          ]
        },
        {
          "id": "d66af6db-a283-4ebc-89ed-ab5f9e65ae07",
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
              "id": "f45811ce-a307-4c6d-b956-58dcf27034a1"
            }
          ]
        },
        {
          "id": "ca46644b-b690-414c-a13e-fed7f95916ad",
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
              "id": "cd77dc7f-e692-49c1-8e91-fd302ba03e93"
            }
          ]
        }
      ]
    },
    {
      "name": "Flag-statuses",
      "item": [
        {
          "id": "bc28b146-b57e-4499-ba00-1e3d67176068",
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
              "id": "7e05b844-5a70-4277-854d-bc3df073e960"
            }
          ]
        },
        {
          "id": "9c934bd5-765a-4a4f-a76f-baf31df194ce",
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
              "id": "7880cd6b-5a07-4f41-98b7-f5eca3ade375"
            }
          ]
        }
      ]
    },
    {
      "name": "Flags",
      "item": [
        {
          "id": "c63f7703-3c8e-44cd-b345-1749c3b1fdbb",
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
              "id": "d7e96838-96dd-4e86-a878-2e3112552333"
            }
          ]
        },
        {
          "id": "3448b37c-4fdf-4444-b34b-c2ff893aecaa",
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
              "id": "bb832e35-e8e7-4e54-9252-75f1fcd0fb9e"
            }
          ]
        },
        {
          "id": "3dea2944-3e65-46ba-a4ed-1f5a0dcd1164",
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
              "id": "033635b2-47b7-41b8-8587-1320c9912315"
            }
          ]
        },
        {
          "id": "9dd084f2-2897-44f9-8215-eb1dcc17be35",
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
              "id": "6b19c67d-1708-4598-a533-ef26f9f7d81c"
            }
          ]
        },
        {
          "id": "fb8da383-d953-4195-a4a0-73391d8b9699",
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
              "id": "9077b388-d356-4c48-b975-a76ce6652bc9"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "73990b2f-2237-4055-a2cf-76f82419c47b",
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
              "id": "9f0a6f8a-a7b6-41a5-9b03-93eafd0a9f71"
            }
          ]
        },
        {
          "id": "0c5736e4-5b39-457e-b873-a06a6643ace7",
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
              "id": "74332691-9c3d-4ec0-ae5e-cddf3c9a8349"
            }
          ]
        }
      ]
    }
  ]
}