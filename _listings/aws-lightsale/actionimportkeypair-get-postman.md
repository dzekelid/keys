{
  "info": {
    "name": "Amazon Lightsale API Import Key Pair",
    "_postman_id": "c0e6d2b4-6e82-440a-9cce-b1a0fe9774c6",
    "description": "Imports a public SSH key from a specific key pair.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "b83ad5d4-75b4-48a5-9c4a-2ddddd24a843",
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
              "id": "ccf7c86f-cff4-4219-825c-28d57c32cf7b"
            }
          ]
        },
        {
          "id": "1477c219-78aa-4e09-a505-85e455f4f6dc",
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
              "id": "f2828451-1965-4ac8-a350-a48d43d676f3"
            }
          ]
        },
        {
          "id": "79fcf6bc-4d26-455d-a4e4-05bfa63838a2",
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
              "id": "ed509437-64d8-4387-933d-e3d3e0bc91b4"
            }
          ]
        },
        {
          "id": "e4ffdcaf-51d6-4dc5-9225-5f28fbf10e22",
          "name": "getStaticIp",
          "request": {
            "url": "http://example.com/api/?Action=GetStaticIp?staticIpName=staticIpName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific static IP."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92d417dd-4205-4602-b05d-9951f222f9f5"
            }
          ]
        },
        {
          "id": "4630fec6-81cc-47b1-9741-5d751e5eafac",
          "name": "getStaticIps",
          "request": {
            "url": "http://example.com/api/?Action=GetStaticIps?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all static IPs in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "121a6119-e6f8-417c-8251-53c53899b121"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "b94fb818-78ef-42e4-801a-100238dd563a",
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
              "id": "c912ade1-8814-48e0-9935-2b9b3e28a145"
            }
          ]
        },
        {
          "id": "dc237d4e-c7c6-4b8f-9340-5534834775e8",
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
              "id": "d8f60c9a-ddfc-474c-ba0b-5b5acf7f882d"
            }
          ]
        },
        {
          "id": "67a605ce-38dc-4943-9c3d-140e36d4f102",
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
              "id": "7f9094bb-a461-4ba2-980b-1de8804958e9"
            }
          ]
        },
        {
          "id": "687e68ec-a315-4716-819d-5f8098c3d554",
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
              "id": "d013373b-7e94-4243-9d0d-b928c8b13c09"
            }
          ]
        },
        {
          "id": "929a8e3f-2038-42e5-a526-9b7dfc50dcd8",
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
              "id": "8457150b-15fe-42de-97aa-3db8238316a5"
            }
          ]
        },
        {
          "id": "df1f102f-961d-49fa-b49e-9cc70ec92734",
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
              "id": "fbb2bbac-1ab8-40df-9398-5add60665969"
            }
          ]
        },
        {
          "id": "558edec7-2f17-437b-a040-bf9e56cd045d",
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
              "id": "5d0845bf-5464-4f1d-8e8f-18a3676be673"
            }
          ]
        },
        {
          "id": "53c9e3f4-a4b4-450d-8c75-25ee63ef8066",
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
              "id": "51ff6885-66de-4c79-aad9-0ccf08668354"
            }
          ]
        },
        {
          "id": "d976ddf8-ea60-4efc-8b18-69ad847a0c0c",
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
              "id": "ea20a23f-771a-4fa8-90a2-7f8567c20973"
            }
          ]
        },
        {
          "id": "49e90d53-f25f-44af-abc6-c39906a3a5f3",
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
              "id": "bcdc2ab9-f01f-494e-8199-29ba36cb7131"
            }
          ]
        },
        {
          "id": "12d4190d-f7c9-4805-a02f-a9ef131c74ab",
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
              "id": "d41d0760-d05c-4567-9886-a202cc73b074"
            }
          ]
        },
        {
          "id": "ec8a508c-3b69-4270-a3d9-03bc4876b748",
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
              "id": "e6c0b519-20bb-4c02-aa82-5d56ddd29242"
            }
          ]
        },
        {
          "id": "47c04df6-8a2b-454f-a447-ad4108701d7a",
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
              "id": "a36fabfe-1422-43d2-9f95-0c8709825101"
            }
          ]
        },
        {
          "id": "a1906265-c498-4d5f-b20c-eac90c2bb068",
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
              "id": "029beaf2-7bd8-4cff-9d79-555eeff86b52"
            }
          ]
        },
        {
          "id": "dc8b92e7-3774-46d7-974a-2c0d8a0cab68",
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
              "id": "dedfa15e-857e-4ed2-8ba4-4a9b4a1aed79"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "8c454a4f-99f3-47ef-82a8-54a557688c8d",
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
              "id": "10885a7c-f022-40d6-bd68-84986d8025f0"
            }
          ]
        },
        {
          "id": "5cf2781e-2d16-4292-a515-cbcce224e50a",
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
              "id": "b7bc4088-7ac4-4e3c-83d0-ae290c7fb922"
            }
          ]
        },
        {
          "id": "345da7c7-6446-49d1-aec5-46988ad262d0",
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
              "id": "ad31e646-5c11-4845-9dda-a5682a0f0a0d"
            }
          ]
        },
        {
          "id": "873c928f-10e8-489f-a1a4-094a34763a3e",
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
              "id": "569099e0-9d5b-416d-ab00-ce0cf9302e81"
            }
          ]
        },
        {
          "id": "e212f580-1f63-45f1-b42a-b19d7edeb294",
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
              "id": "5bd24c1d-eb09-471c-b74c-d56b9ffdde93"
            }
          ]
        },
        {
          "id": "88d27261-3e6c-42e8-a5e6-d1ec5e1ff949",
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
              "id": "6ecb0ef9-d00e-4710-bcb2-19d55ffb9d29"
            }
          ]
        }
      ]
    },
    {
      "name": "Key Pairs",
      "item": [
        {
          "id": "eb6adc6e-8c8f-4b16-ae57-50bfbd9e5e29",
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
              "id": "207f72ef-a196-4176-a895-de136fe27c60"
            }
          ]
        },
        {
          "id": "44fd2545-f10f-4d5d-935c-92923609ee0d",
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
              "id": "726cd651-fe40-473d-8067-9c83398d4e6c"
            }
          ]
        },
        {
          "id": "e5b2a6d2-6002-4593-9303-db5b5352a566",
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
              "id": "d86a1a97-419d-4b57-8609-94b5241d297b"
            }
          ]
        },
        {
          "id": "8665b763-5e75-496f-8a2d-e3a0cb224b1e",
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
              "id": "1dd45e68-b27b-4218-a0a3-541e11aaf353"
            }
          ]
        },
        {
          "id": "0c34cf7c-d563-4954-8204-a91c16b00bbc",
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
              "id": "dd1d7d51-82b7-4749-a822-f653f6ddff0c"
            }
          ]
        },
        {
          "id": "5bb7049a-425a-4a24-8d92-b7a3aceefa15",
          "name": "importKeyPair",
          "request": {
            "url": "http://example.com/api/?Action=ImportKeyPair?keyPairName=keyPairName&publicKeyBase64=publicKeyBase64",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Imports a public SSH key from a specific key pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3654538-fb0f-46fa-accb-4ec9768d26d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Names",
      "item": [
        {
          "id": "45936c49-cfcc-4dc0-979e-94759529f3db",
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
              "id": "827378bd-ed12-4d0f-9130-86f6e97043c6"
            }
          ]
        }
      ]
    },
    {
      "name": "Bundles",
      "item": [
        {
          "id": "d8eb40b7-3f55-44ec-9310-abd38c382d9f",
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
              "id": "c3d3fa5b-713b-4581-bbb3-c02c6e68e896"
            }
          ]
        }
      ]
    },
    {
      "name": "Operations",
      "item": [
        {
          "id": "46fe291e-f3bb-46bb-a560-7a892fcbd744",
          "name": "getOperation",
          "request": {
            "url": "http://example.com/api/?Action=GetOperation?operationId=operationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specific operation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41a3519f-67f4-4e75-b7a1-211a271ce9e5"
            }
          ]
        },
        {
          "id": "efb01892-6ca7-4d40-a7ef-9f562b8ec1b9",
          "name": "getOperations",
          "request": {
            "url": "http://example.com/api/?Action=GetOperations?pageToken=pageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about all operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb5de900-5a36-4715-996b-406ccb42c510"
            }
          ]
        },
        {
          "id": "17ee0f38-0451-4bf7-940e-13c09fa57898",
          "name": "getOperationsForResource",
          "request": {
            "url": "http://example.com/api/?Action=GetOperationsForResource?pageToken=pageToken&resourceName=resourceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets operations for a specific resource (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9182d97-1504-42d8-8118-f0a2992de491"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "f7cc3656-aaef-4bb8-9dfe-19e867227334",
          "name": "getRegions",
          "request": {
            "url": "http://example.com/api/?Action=GetRegions?includeAvailabilityZones=includeAvailabilityZones",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all valid regions for Amazon Lightsail."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45478493-bdaf-48e1-a47e-a00220639c0f"
            }
          ]
        }
      ]
    }
  ]
}