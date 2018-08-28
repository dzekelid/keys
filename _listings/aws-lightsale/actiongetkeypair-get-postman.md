{
  "info": {
    "name": "Amazon Lightsale API Get Key Pair",
    "_postman_id": "730f6572-1864-4de7-8639-2a5e20c79c3f",
    "description": "Returns information about a specific key pair.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "af9afae2-cc6c-4e44-95d2-3bfd6583aa4f",
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
              "id": "4b384182-8462-4438-b399-1c805b07f66b"
            }
          ]
        },
        {
          "id": "7502357a-cd08-4a8c-9883-398ada649cd2",
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
              "id": "892ee93a-bb7b-4bb9-85f5-5d13cbe8e5a6"
            }
          ]
        },
        {
          "id": "a5e0a560-8cbe-4e83-8b15-9f3aefcca50f",
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
              "id": "0140e579-6744-4463-9c6f-aa2e896116d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "0ef2fa6f-b5e6-4126-bcc4-19df5ca16f23",
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
              "id": "3edd32f8-7016-44dd-b09e-0c8583e618d1"
            }
          ]
        },
        {
          "id": "faa3341c-014d-4788-9ab6-7b5700a6ca79",
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
              "id": "7b7978f9-36b1-4b3e-ac10-86b84efa5cb1"
            }
          ]
        },
        {
          "id": "1390d9f6-6d99-48ca-b19d-c8735da509f9",
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
              "id": "6c14c55f-c80c-4375-bbe3-48b62cef5d03"
            }
          ]
        },
        {
          "id": "156738bd-f42e-4f08-a3b5-9af432cd5a18",
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
              "id": "e626ba4c-487e-4a8e-a756-ce0c9d859576"
            }
          ]
        },
        {
          "id": "7379649a-f9f6-447d-8b86-dabae775ed35",
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
              "id": "b33eb240-97fa-4354-bf6d-c8091fa6c285"
            }
          ]
        },
        {
          "id": "02e9222b-1768-46b1-b07a-5877f4e63e69",
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
              "id": "ff87b44e-d605-4c20-baa6-0715cc2d36cd"
            }
          ]
        },
        {
          "id": "6b16abb6-a6c3-47d0-8a21-b3a85b98ce20",
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
              "id": "2cafd80c-a401-4f25-9637-04faf918c487"
            }
          ]
        },
        {
          "id": "368ee49e-5def-4a70-b4cc-ef4d781cc0ed",
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
              "id": "0181537f-f1f6-4bc9-aa71-636533c8bea2"
            }
          ]
        },
        {
          "id": "e7ff4d6a-64fc-4810-9dc0-958904860438",
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
              "id": "9965c338-5d08-4e2e-8e99-76321cd2aaad"
            }
          ]
        },
        {
          "id": "5862ca5f-0ca2-4319-b75a-51a4279f7413",
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
              "id": "183cd1f8-2318-4179-b983-8d9f53da62bd"
            }
          ]
        },
        {
          "id": "8262e78d-b0f6-44b3-b5f0-cee3b85d517f",
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
              "id": "497e350e-1683-4ee4-b82f-5dc22512c9ca"
            }
          ]
        },
        {
          "id": "4b61be9c-b423-4b94-88e3-d693e460d135",
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
              "id": "9c3d8110-8cae-4c7b-a69f-a0e2fb9bfb0d"
            }
          ]
        },
        {
          "id": "de212ff4-2fd5-442e-8c8c-7f6f344da788",
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
              "id": "c9eda3e7-9f0e-4a56-ab9a-0fb26db3e9f5"
            }
          ]
        },
        {
          "id": "d1465ab4-4b36-4942-9325-a879c384837b",
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
              "id": "664d58a3-3eaa-4328-928e-a9d689f104af"
            }
          ]
        },
        {
          "id": "dae0c831-75f9-4136-a2e7-1bea6905ba63",
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
              "id": "98797284-2bc2-4a21-8fa6-bbc9e9dfd95d"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "1e53d407-07f4-4210-8413-602160545a45",
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
              "id": "9ffaae6a-90da-4e7e-a033-a4472094212f"
            }
          ]
        },
        {
          "id": "42821122-78ee-48bd-844d-005d1caee094",
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
              "id": "0725dbd4-150d-492b-acb0-6868b45d2af1"
            }
          ]
        },
        {
          "id": "b1459810-7125-4e2b-ad04-24a3540aa1ea",
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
              "id": "a8669e1b-1d76-44f6-b1a1-0f26bce594f1"
            }
          ]
        },
        {
          "id": "16e3c027-9e2e-4933-ad3c-6b028678b138",
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
              "id": "9f566c66-30b6-436f-9361-aad2f050fdc0"
            }
          ]
        },
        {
          "id": "6c63d7cd-68ff-4a49-b867-5702d1d9a0e8",
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
              "id": "989fa60e-e4af-4093-8c4c-b016fb1245a5"
            }
          ]
        },
        {
          "id": "cec978e0-d573-4b5f-a3f9-380c207d024c",
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
              "id": "893952f1-3244-4b9b-8c02-1cbeb4f39e9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Key Pairs",
      "item": [
        {
          "id": "36684fd2-6ff6-47fc-b48a-9da0a1497585",
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
              "id": "b3e40427-8703-4720-8591-0c929badba8f"
            }
          ]
        },
        {
          "id": "42c12680-4f1f-4ec4-871e-c7648f292576",
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
              "id": "6237ca69-479e-448d-875b-ed82a0c53e7d"
            }
          ]
        },
        {
          "id": "c7f85984-c5f6-463d-8c38-9d8280ae639b",
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
              "id": "810efaed-6bcd-4085-9890-754f770f743d"
            }
          ]
        },
        {
          "id": "7e7aed49-bda7-40e6-bcf5-991ca21b5047",
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
              "id": "5fbbcaf7-e496-4eeb-af7b-d21364b03bba"
            }
          ]
        }
      ]
    },
    {
      "name": "Names",
      "item": [
        {
          "id": "aa9e99f6-da3d-4953-9244-468bcd03f04b",
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
              "id": "e021378d-cab4-438b-b7b6-e2de2db5e02a"
            }
          ]
        }
      ]
    },
    {
      "name": "Bundles",
      "item": [
        {
          "id": "949d3536-1507-4e44-a94d-2768029a1f37",
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
              "id": "fdce733d-0786-4c16-8ec0-50b26fe1ae67"
            }
          ]
        }
      ]
    }
  ]
}