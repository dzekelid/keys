{
  "info": {
    "name": "Amazon Lightsale API Get Key Pairs",
    "_postman_id": "6545fc81-bcbe-4a7a-adbd-0693140d03cf",
    "description": "Returns information about all key pairs in the user's account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "111866c8-0368-4083-aba2-8e5b44e1e36e",
          "name": "allocateStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=AllocateStaticIp?staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allocates a static IP address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b93ab396-bfb9-480c-b146-1971f6ea7846"
            }
          ]
        },
        {
          "id": "a1876aa4-3132-4dbd-9f0d-c6d5b13271cf",
          "name": "attachStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=AttachStaticIp?instanceName=instanceName&staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches a static IP address to a specific Amazon Lightsail instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "520df6c8-7c51-4c4d-a397-f6b382b85631"
            }
          ]
        },
        {
          "id": "4561ffdd-f23a-436f-94da-d926c4fe5495",
          "name": "detachStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=DetachStaticIp?staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches a static IP from the Amazon Lightsail instance to which it is\n      attached."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05abfa10-5ddf-4488-9831-5c8d6c9c0ed3"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "869e3fac-8350-4730-8298-8b4d899e4ad8",
          "name": "closeInstancePublicPorts",
          "request": {
            "url": "http://example.com/api/?Action=CloseInstancePublicPorts?instanceName=instanceName&portInfo=portInfo",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Closes the public ports on a specific Amazon Lightsail instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8afe5aee-5734-4eee-ae63-86aca37ed078"
            }
          ]
        },
        {
          "id": "c21b06f4-48e9-45ca-80d1-1b4aad0a4555",
          "name": "createInstances",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstances?availabilityZone=availabilityZone&blueprintId=blueprintId&bundleId=bundleId&customImageName=customImageName&instanceNames=instanceNames&keyPairName=keyPairName&userData=userData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates one or more Amazon Lightsail virtual private servers, or\n        instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55c0b1ce-1082-4595-8da8-1db834922f9c"
            }
          ]
        },
        {
          "id": "a33cbd91-1f70-4812-a805-76fde7cb0d5e",
          "name": "createInstancesFromSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstancesFromSnapshot?availabilityZone=availabilityZone&bundleId=bundleId&instanceNames=instanceNames&instanceSnapshotName=instanceSnapshotName&keyPairName=keyPairName&userData=userData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uses a specific snapshot as a blueprint for creating one or more new instances that are\n      based on that identical configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d38276a6-7690-4696-a037-99c9d63e1eb8"
            }
          ]
        },
        {
          "id": "c34de793-50f6-458d-a17f-829c4bdb0918",
          "name": "createInstanceSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstanceSnapshot?instanceName=instanceName&instanceSnapshotName=instanceSnapshotName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a specific virtual private server, or\n        instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ed30946-445d-432e-82c2-2e3ffb7eb78b"
            }
          ]
        },
        {
          "id": "99f28da2-8ac4-401b-a8dc-ebbc4d2edeb6",
          "name": "deleteInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInstance?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific Amazon Lightsail virtual private server, or\n        instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51a78457-215a-409f-a7d3-b2d89e6416eb"
            }
          ]
        },
        {
          "id": "613b10bd-48b9-4fae-bc79-6c1b438ab638",
          "name": "deleteInstanceSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInstanceSnapshot?instanceSnapshotName=instanceSnapshotName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific snapshot of a virtual private server (or\n        instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50a49b92-5f53-4a21-9271-608c7736691a"
            }
          ]
        },
        {
          "id": "d092e44f-b19d-4a46-83fc-fa23f66dce33",
          "name": "getBlueprints",
          "request": {
            "url": "http://example.com/api/?Action=GetBlueprints?includeInactive=includeInactive&pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of available instance images, or blueprints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92b6394f-56f1-485d-9069-af147dac94fe"
            }
          ]
        },
        {
          "id": "df2253e6-f846-49dd-aa08-f505201ab4dc",
          "name": "getInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetInstance?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific Amazon Lightsail instance, which is a virtual\n      private server."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69e449db-fa53-49e7-9f54-650d689de7c3"
            }
          ]
        },
        {
          "id": "0a3a1cbc-fa1a-4cab-9a45-f87d688c5b0f",
          "name": "getInstanceAccessDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceAccessDetails?instanceName=instanceName&protocol=protocol",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns temporary SSH keys you can use to connect to a specific virtual private server,\n      or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb0ec52d-1290-4965-97f1-548ee7b049e7"
            }
          ]
        },
        {
          "id": "4d2c9813-43e9-4ba0-b0f9-de45c0fac097",
          "name": "getInstanceMetricData",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceMetricData?endTime=endTime&instanceName=instanceName&metricName=metricName&period=period&startTime=startTime&statistics=statistics&unit=unit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the data points for the specified Amazon Lightsail instance metric, given an\n      instance name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "580294da-8fe4-4f80-9967-a14943e2338c"
            }
          ]
        },
        {
          "id": "ce15651e-49f3-4b27-aa56-108ae539bd92",
          "name": "getInstancePortStates",
          "request": {
            "url": "http://example.com/api/?Action=GetInstancePortStates?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the port states for a specific virtual private server, or\n        instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ddfd94c-59f1-43a8-b2df-d8e318105bfd"
            }
          ]
        },
        {
          "id": "a21ec69a-5130-420d-8092-542e8533dec2",
          "name": "getInstances",
          "request": {
            "url": "http://example.com/api/?Action=GetInstances?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all Amazon Lightsail virtual private servers, or\n        instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdba5745-19be-4125-9165-043eae13b365"
            }
          ]
        },
        {
          "id": "0e8b1665-5410-42d5-a9ab-72be91c2512f",
          "name": "getInstanceSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceSnapshot?instanceSnapshotName=instanceSnapshotName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific instance snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a53a48b6-f0f1-4f2e-ac44-65356c8be57a"
            }
          ]
        },
        {
          "id": "81cda8fa-dda4-49ff-8e78-60922eb737a0",
          "name": "getInstanceSnapshots",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceSnapshots?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all instance snapshots for the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66c6d3b1-2ffc-4c96-bacc-c8b016602fd9"
            }
          ]
        },
        {
          "id": "9bb70bf3-2502-41a8-8432-1360b9b75baa",
          "name": "getInstanceState",
          "request": {
            "url": "http://example.com/api/?Action=GetInstanceState?instanceName=instanceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the state of a specific instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87eab2a8-3ab2-47d6-a0c6-73587f07aa1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "03914600-1fbd-4ae7-85b3-88dec8eaea9b",
          "name": "createDomain",
          "request": {
            "url": "http://example.com/api/?Action=CreateDomain?domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a domain resource for the specified domain (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59dc96bf-8aa3-4e35-b18d-b43d55e7c00a"
            }
          ]
        },
        {
          "id": "463ac93d-8c9d-457f-af6e-c2d88623f69f",
          "name": "createDomainEntry",
          "request": {
            "url": "http://example.com/api/?Action=CreateDomainEntry?domainEntry=domainEntry&domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates one of the following entry records associated with the domain: A record, CNAME\n      record, TXT record, or MX record."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f0c1a42-56fb-4eb6-a163-0da1c1f51ba0"
            }
          ]
        },
        {
          "id": "ce1f474d-c49d-4e07-9318-601df7a9a460",
          "name": "deleteDomain",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDomain?domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified domain recordset and all of its domain records."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc3f2195-fd58-4a13-b554-fab4358fccd4"
            }
          ]
        },
        {
          "id": "d49e96d2-7caf-4bb2-825a-1e4835ce8402",
          "name": "deleteDomainEntry",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDomainEntry?domainEntry=domainEntry&domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific domain entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b675aaab-9b42-4a0a-a117-e2ed19397d18"
            }
          ]
        },
        {
          "id": "d0cf0b72-a0a2-4f7a-955a-8bc7762832d1",
          "name": "getDomain",
          "request": {
            "url": "http://example.com/api/?Action=GetDomain?domainName=domainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific domain recordset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bfaece5-9f49-4bdd-9a7c-31a144679aa1"
            }
          ]
        },
        {
          "id": "327073e0-0e75-4a41-b788-4c39b03ff363",
          "name": "getDomains",
          "request": {
            "url": "http://example.com/api/?Action=GetDomains?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all domains in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c56e0331-a551-4f56-83ae-1cfdd8d052c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Key Pairs",
      "item": [
        {
          "id": "d539026d-45c2-4dc0-86cc-51903a7631e8",
          "name": "createKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=CreateKeyPair?keyPairName=keyPairName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates sn SSH key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69c058d5-25a3-4973-a850-b59ff381df07"
            }
          ]
        },
        {
          "id": "1ad4fc67-d121-48f5-aabe-885ca9758291",
          "name": "deleteKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=DeleteKeyPair?keyPairName=keyPairName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific SSH key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6a43c1e-ccd6-4161-8be9-6b0a4e759299"
            }
          ]
        },
        {
          "id": "4af37234-4352-4f5a-a5f2-e4cdee0b2104",
          "name": "downloadDefaultKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=DownloadDefaultKeyPair?privateKeyBase64=privateKeyBase64&publicKeyBase64=publicKeyBase64",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Downloads the default SSH key pair from the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dab36b40-ca93-4db0-b28e-30125fed6772"
            }
          ]
        },
        {
          "id": "93d2f707-ca75-4adf-a6c4-feba0d00d5fe",
          "name": "getKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=GetKeyPair?keyPairName=keyPairName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0c999af-54bf-4e48-a9d3-268082994b64"
            }
          ]
        },
        {
          "id": "0519e9ec-853a-4322-8247-4e86b6fbc49a",
          "name": "getKeyPairs",
          "request": {
            "url": "http://example.com/api/?Action=GetKeyPairs?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all key pairs in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d47df8af-61b5-467d-9d76-8b41338477ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Names",
      "item": [
        {
          "id": "2bb47444-cdf6-4a59-beb2-292a0f73bf90",
          "name": "getActiveNames",
          "request": {
            "url": "http://example.com/api/?Action=GetActiveNames?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the names of all active (not deleted) resources."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a589d7b6-4150-4a62-abe4-e31ab1f28225"
            }
          ]
        }
      ]
    },
    {
      "name": "Bundles",
      "item": [
        {
          "id": "c811f345-7e3c-4e69-a038-ed3a0987014c",
          "name": "getBundles",
          "request": {
            "url": "http://example.com/api/?Action=GetBundles?includeInactive=includeInactive&pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of bundles that are available for purchase."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2b2f02f-3b1c-4fac-baa2-8197e707f23d"
            }
          ]
        }
      ]
    }
  ]
}