{
  "info": {
    "name": "Amazon Lightsale API Create Key Pair",
    "_postman_id": "9efdcd33-d153-4bc2-966b-d70478f523bb",
    "description": "Creates sn SSH key pair.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "8d93f59a-5810-4750-8d4f-bf13bda7fb36",
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
              "id": "e00ae893-b525-489e-873b-e001bff1e01d"
            }
          ]
        },
        {
          "id": "e5332ab8-1ac4-41d5-b472-e3709c16c327",
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
              "id": "72e172d1-9969-472b-9a7d-7874106b10ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "e1661289-b78f-4f45-b114-8a3c0ca033e5",
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
              "id": "ab83412f-9069-4e78-ab56-146ed600b0e7"
            }
          ]
        },
        {
          "id": "28cce9c0-df7c-44ba-8501-553faf9025d8",
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
              "id": "24acceca-d3ae-4267-8b29-30795679d24f"
            }
          ]
        },
        {
          "id": "7e0a741b-e39f-41ce-9d58-d4878ebd5daf",
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
              "id": "1e23aa77-4fa9-4c3b-a0fd-95be22f35676"
            }
          ]
        },
        {
          "id": "19f2a560-7689-436e-b2f8-1e9d046982bf",
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
              "id": "876d25b4-7795-4944-b792-53208e144cc3"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "302a6bce-2a40-4307-bc04-b1fc1ac77cfe",
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
              "id": "14056006-3d81-48e4-afc0-737cfa2b48fe"
            }
          ]
        },
        {
          "id": "147ed4da-9e72-4816-87bf-21e6c973fbde",
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
              "id": "89c555a7-2c16-43b1-b44c-66647f34b871"
            }
          ]
        }
      ]
    },
    {
      "name": "Key Pairs",
      "item": [
        {
          "id": "7b5b8b8f-a6e7-4f57-8168-b70ec81ccd80",
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
              "id": "90063021-8687-4f08-aafc-0b3a25e7b05e"
            }
          ]
        }
      ]
    }
  ]
}