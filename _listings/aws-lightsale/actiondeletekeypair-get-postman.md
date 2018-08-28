{
  "info": {
    "name": "Amazon Lightsale API Delete Key Pair",
    "_postman_id": "d6904b5b-f6ab-4b3c-a318-d2402aba0f7a",
    "description": "Deletes a specific SSH key pair.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "c8bdd080-a911-4651-81a4-0b198e647cc7",
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
              "id": "08d27cbf-83dc-464c-b86a-3178179401e6"
            }
          ]
        },
        {
          "id": "d03ebf8a-76e4-459a-a7e4-9a96744d8ea7",
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
              "id": "d573ac48-c457-4060-b477-597ccff929fd"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "29213f86-cf4c-43b6-a75d-cb32f2b13f0a",
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
              "id": "33971129-076d-4493-8dcf-ac5a7df9b113"
            }
          ]
        },
        {
          "id": "ccfc0622-bf13-4427-870b-456b6d50bda7",
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
              "id": "7db574b2-d88f-4df5-aad4-77ab6d19312a"
            }
          ]
        },
        {
          "id": "a52bb63b-7173-4b74-af81-f3e1a0246e03",
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
              "id": "35c6c747-3b66-4fbe-ae97-2c0651b14bd0"
            }
          ]
        },
        {
          "id": "3f96b867-7b78-47f6-b30a-d0d27c0ec2ef",
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
              "id": "f9b808fa-c178-49c4-8010-80450182ff9f"
            }
          ]
        },
        {
          "id": "0e150cc8-0944-4f55-87bf-d83a06abb9c2",
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
              "id": "1cd95a87-f53d-451c-a858-433b04dbb2ee"
            }
          ]
        },
        {
          "id": "1850f9cc-60d9-46c6-8e9c-1ab6b577802e",
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
              "id": "9ae1505e-bfe1-448c-8054-33600c416063"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "1bcdc2f6-ad8e-4c32-b0fd-3dd39ae7a829",
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
              "id": "93c1b2c7-0af5-4dab-b79f-47b79ff80c3a"
            }
          ]
        },
        {
          "id": "498baa28-67b6-450e-bc25-4a36dfd30d09",
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
              "id": "59199e38-96b4-4da4-8a2c-cd178cdc6ca1"
            }
          ]
        },
        {
          "id": "c50ca279-fa59-4ba4-a885-d24f0fa2a0e1",
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
              "id": "0c982e84-5f7f-4a85-bf08-3e62845b39a3"
            }
          ]
        },
        {
          "id": "1b13989d-234a-43a5-8b70-3c0b3ce89259",
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
              "id": "ccfd2b0c-0692-4394-9839-9b4804b2249a"
            }
          ]
        }
      ]
    },
    {
      "name": "Key Pairs",
      "item": [
        {
          "id": "f710377f-17a1-47db-93ec-e994ce443cb9",
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
              "id": "9b7f4132-cd96-4a22-b5cd-dfe28703987b"
            }
          ]
        },
        {
          "id": "41ed8ed3-0bad-41eb-b2f5-178d2d6e01ff",
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
              "id": "758ea650-ab6c-4e9c-b76d-71a58c1d2b4c"
            }
          ]
        }
      ]
    }
  ]
}