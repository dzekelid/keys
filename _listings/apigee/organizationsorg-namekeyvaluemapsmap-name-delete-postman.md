{
  "info": {
    "name": "Apigee Edge Delete Organizations Name Keyvaluemaps Map Name",
    "_postman_id": "0e3269df-10e2-4e4c-a1d4-086a684d9752",
    "description": "Deletes a KeyValueMap and all associated entries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "34fb92d8-9596-489a-af9a-6fb08259c98c",
          "name": "getOrganizations",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/organizations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the organizations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9251fcc3-7c66-4b94-b370-922034c8cbec"
            }
          ]
        },
        {
          "id": "78bc4c18-9d9b-4cea-9087-6bc0e5627e63",
          "name": "postOrganizations",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/organizations?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5eec7f6b-ecdd-4f64-ae09-f4c29d5ec6e8"
            }
          ]
        },
        {
          "id": "69bffa35-4288-4733-ae8a-e95392d91405",
          "name": "getOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f3292c8-c149-4392-b7d6-f47c0cecf129"
            }
          ]
        },
        {
          "id": "1a1e4716-3cb3-45fc-8b67-d248d76fbca9",
          "name": "putOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the description of a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "031e0ccc-e785-46f2-865b-23ed145ef049"
            }
          ]
        },
        {
          "id": "6c2a5bbd-15ea-407e-bda8-7e933cc923f7",
          "name": "deleteOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b21f025-00e8-4099-8037-46bfce40b4e5"
            }
          ]
        },
        {
          "id": "a10078e0-e413-4054-a097-bddd0dfd2adc",
          "name": "getOrganizationsOrgNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/deployments"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all deployments of an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65db7b47-418a-47f5-9b75-d9ed98173441"
            }
          ]
        },
        {
          "id": "36e7d150-1364-4a42-9472-9543992a9d97",
          "name": "getOrganizationsOrgNamePods",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/pods"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pods associated with an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3367b0cb-378a-4518-a60d-fbe35fee0075"
            }
          ]
        },
        {
          "id": "d62e24d6-d065-4496-8dac-52e98fea94b9",
          "name": "postOrganizationsOrgNamePods",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/pods"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates a pod from an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6813a6d-74a9-482d-ae97-612fed23e58a"
            }
          ]
        },
        {
          "id": "c8e83540-b634-49b0-9fce-d57951d92672",
          "name": "getOrganizationsOrgNameEnvironments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the environments in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "840dbf3f-5623-41f6-89b4-8e3df7a46a71"
            }
          ]
        },
        {
          "id": "3a950ddf-ba0b-4a95-aa85-980fbab49559",
          "name": "postOrganizationsOrgNameEnvironments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb06fd49-9035-4c10-b4c1-bbc0c2a2b844"
            }
          ]
        },
        {
          "id": "4b82e155-d9cd-45e2-880e-6d9e598f86da",
          "name": "getOrganizationsOrgNameEnvironmentsEnvName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details for an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dd67357-6971-41c6-81a4-c50688ee6b30"
            }
          ]
        },
        {
          "id": "e5b6aa25-472e-4feb-ac2a-92e7273712c9",
          "name": "postOrganizationsOrgNameEnvironmentsEnvName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd61601b-3d3c-4564-894d-513ab7a90fa8"
            }
          ]
        },
        {
          "id": "21c4b8aa-2a26-468b-9a5e-f512a25c7874",
          "name": "deleteOrganizationsOrgNameEnvironmentsEnvName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bd312ef-1c84-408f-b4af-59243d7104db"
            }
          ]
        },
        {
          "id": "bebbe96f-2fc2-4150-9a79-905e6cc7f738",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/deployments"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the deployments for an environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3446c556-d7b6-4526-aeb9-1624585bb7fb"
            }
          ]
        },
        {
          "id": "66c72a0b-df39-42ea-b9f6-d437301a9c3a",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameApisApiNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/apis/:api_name/deployments"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the deployments for an API Proxy in the given environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d82b5aae-ca5d-4141-ac63-22befa1296f8"
            }
          ]
        },
        {
          "id": "57ec6999-b43b-4c8d-b574-7bde55739d2a",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameApisApiNameRevisionsRevisionNumberDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/apis/:api_name/revisions/:revision_number/deployments"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "revision_number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the deployments for an API Proxyâ????s revision for an environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7b7a0fb-a7e5-4288-b3c9-796f6f484488"
            }
          ]
        },
        {
          "id": "35f87dc9-4f49-491f-b7b3-fd54124b259f",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameServers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/servers"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the servers that are bound to an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84eff8d7-c80c-487f-98e6-67b86533369a"
            }
          ]
        },
        {
          "id": "3b95814b-e1ab-4864-8c87-4022f4dd544c",
          "name": "postOrganizationsOrgNameEnvironmentsEnvNameServers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/servers"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add servers into the environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d3bc3c4-e327-415d-bd01-32cf1c151377"
            }
          ]
        },
        {
          "id": "8ec7db8b-ae3f-4a78-901f-3df8c83a2468",
          "name": "deleteOrganizationsOrgNameEnvironmentsEnvNameServers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/servers"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes servers from the environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc4700db-1173-4331-8b2d-e96fa581358b"
            }
          ]
        },
        {
          "id": "d3c48fc3-e499-4f41-bb4d-a015631d8a74",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameVirtualhosts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all virtual hosts in an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58d84e17-dee3-41a3-8c51-b4bdf2e3a808"
            }
          ]
        },
        {
          "id": "bb1613a9-b6df-4a2c-91b7-65c12ba6a01c",
          "name": "postOrganizationsOrgNameEnvironmentsEnvNameVirtualhosts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a virtual host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef347411-c1bd-46b4-84e0-e022a5d50fc0"
            }
          ]
        },
        {
          "id": "74e51aa5-1761-4acc-84c5-cd5beba3343c",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts/:virtualhost_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualhost_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details for a named virtual host ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c59970ec-9e32-4cb1-b51a-85a6d1c40b55"
            }
          ]
        },
        {
          "id": "2b2ad1f0-0fc3-4376-94ce-c560cc8efea7",
          "name": "postOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts/:virtualhost_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualhost_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a specific virtual host in an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f894451-858b-4f80-a52c-06f0884195b1"
            }
          ]
        },
        {
          "id": "144f59db-68dd-4c89-8457-d51a804bf853",
          "name": "deleteOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts/:virtualhost_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualhost_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific virtual host in an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ba86887-d1a9-4408-907f-df7e845adf06"
            }
          ]
        },
        {
          "id": "80e0ce16-ff12-41af-8ad3-823d34dd77d9",
          "name": "getOrganizationsOrgNameApis",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all APIs in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8ab699f-e796-4812-9b6e-520ab7b8a718"
            }
          ]
        },
        {
          "id": "a5797b25-a123-4508-b943-317275977760",
          "name": "postOrganizationsOrgNameApis",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads a ZIP-formatted API proxy configuration bundle from a local machine to an organization on the API Platform."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a190b7e-3866-43a1-b03a-66a6d7ebf4eb"
            }
          ]
        },
        {
          "id": "54f0fc1f-1822-465a-b027-02c0d5cbd6cb",
          "name": "getOrganizationsOrgNameApiproducts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all API products by name for an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab35e180-3d07-4883-a395-4395ba4f9d29"
            }
          ]
        },
        {
          "id": "94ab7b8e-d634-4b48-bec6-908acb53b438",
          "name": "postOrganizationsOrgNameApiproducts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an API product: a list of API resources combined with Quota settings that you can use to deliver customized API bundles to your developers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0567c00f-a203-4388-aa43-821316f7ee0b"
            }
          ]
        },
        {
          "id": "dc617085-3284-467e-b11b-9e8a96f4d79c",
          "name": "getOrganizationsOrgNameApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts/:apiproduct_name"
              ],
              "query": [
                {
                  "key": "entity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "query",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the list of keys/apps/developers for an API product of an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6e568d1-fbe8-4d01-8765-81d0fef55a1e"
            }
          ]
        },
        {
          "id": "ace5c08f-4c2a-4d35-8815-5284efc2a918",
          "name": "putOrganizationsOrgNameApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts/:apiproduct_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "This method updates an existing API product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a09c3b45-5e20-46fc-a321-50626f5002fe"
            }
          ]
        },
        {
          "id": "53e39695-810d-4215-bc41-ddb30ee276be",
          "name": "deleteOrganizationsOrgNameApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts/:apiproduct_name"
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an API product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd9ffad5-0af9-4422-ae0a-aee82335827a"
            }
          ]
        },
        {
          "id": "51444547-4fdb-42a1-8d81-1b9c5543ae84",
          "name": "getOrganizationsOrgNameDevelopers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers"
              ],
              "query": [
                {
                  "key": "registeredat",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the developer profile by registered date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29e29e27-5567-4a33-a6f4-a0158129e320"
            }
          ]
        },
        {
          "id": "7dcfb78d-2a4b-4bd6-88eb-d121fca4c516",
          "name": "postOrganizationsOrgNameDevelopers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a developer in an organization ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5143daf6-2aff-4373-be83-efae1af7edc9"
            }
          ]
        },
        {
          "id": "ece98962-6544-4058-8974-6b2e0b85a203",
          "name": "getOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "query": [
                {
                  "key": "entity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "query",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a count of apps by developer email address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8900d52d-caee-4f95-b502-9f0f30a1ce5f"
            }
          ]
        },
        {
          "id": "c8c6e486-5543-46cc-94f4-4e3e3ff78428",
          "name": "putOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing developer profile with new values or additional attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36917d51-de89-4422-a068-0bbbb926a98d"
            }
          ]
        },
        {
          "id": "ac0c7a61-37e8-497a-a8c2-46d152bc60a1",
          "name": "postOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the status of a developer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3371e5da-7aa8-43b6-9dee-6d1f16b85657"
            }
          ]
        },
        {
          "id": "e2c00d3e-4d17-4058-bedb-a58d4bdb5ad5",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a developer from an Organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc421792-9318-4186-8488-a8419754a5a0"
            }
          ]
        },
        {
          "id": "14a63160-996b-43b5-b964-9fbbefae53f3",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailApps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides an expanded view of a developer's collection of apps ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "562fe08d-20e7-4959-9a18-32dac2c4cafc"
            }
          ]
        },
        {
          "id": "3fb8b66c-c24a-4cd5-b674-bade7ac74bf2",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailApps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app associated with a developer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9b0a418-38dc-423d-8b46-79b43732352e"
            }
          ]
        },
        {
          "id": "17c759dc-0657-4a31-88f6-2dda8dad539f",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "query": [
                {
                  "key": "entity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "query",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a count of all API resources in the API products accessible by a developer app ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b376b13-6576-4387-b15f-8dd903ea233a"
            }
          ]
        },
        {
          "id": "3d2c6644-e5d8-480b-856c-3b3fcfa909dc",
          "name": "putOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the app to get a new set of consumer credentials."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12977da1-be91-4b9d-ab49-98bf3a49c8ee"
            }
          ]
        },
        {
          "id": "2402f9c8-0ab3-4e8e-9472-279795897a92",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes a Developer App, disabling access to all API Products ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be648158-9725-400e-976b-effe19f092d5"
            }
          ]
        },
        {
          "id": "0f236a48-7ab6-408f-a27f-5fda89584b3a",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a Developer's App."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "650b7c0b-bb80-468c-973f-e3895496f5c4"
            }
          ]
        },
        {
          "id": "80981605-0f2a-486f-a715-c73e0ceff8a2",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details for a consumer key for a developer app ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d4fefb6-f149-4dbf-829a-0ab767b5194c"
            }
          ]
        },
        {
          "id": "754bd464-ba2b-44cf-997a-f4a62df02bd1",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes a developer app key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19add24c-c7b4-4269-82aa-22170cf0d11c"
            }
          ]
        },
        {
          "id": "2018f9b3-e554-47ce-8231-e75e8bd71c0b",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a consumer key that belongs to an app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d94d9715-0413-4999-acbb-e2580047d2f2"
            }
          ]
        },
        {
          "id": "96a5696b-0afd-4fa0-8718-33c7a374406e",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key/apiproducts/:apiproduct_name"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes the association of an API Product with a Developer App's consumer key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9f6b770-4904-46f4-bc26-2c5d332fa2d7"
            }
          ]
        },
        {
          "id": "6a48a977-9ad3-433d-8c42-f1f63832f15c",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductNam",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key/apiproducts/:apiproduct_name"
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an API product from a developer app key profile, and thereby renders the developer app unable to access the URIs defined in the API product specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bada4ef-0ca4-4f52-9ac5-686a66c1725e"
            }
          ]
        },
        {
          "id": "73fefd13-179d-4f3e-819f-adaf0e1a4f6c",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth1accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/oauth1accesstokens"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get count of OAuth 1.0 access tokens for a developer's app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05bd2369-5c2f-4d34-9362-9fe5d18b656b"
            }
          ]
        },
        {
          "id": "7bcd141e-2565-4a62-bbaa-eb6ef7a97ae0",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth2accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee