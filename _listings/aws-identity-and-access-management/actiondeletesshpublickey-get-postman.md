{
  "info": {
    "name": "AWS Identity and Access Management API Delete S S H Public Key",
    "_postman_id": "de1ef423-2e01-4cd9-9958-fafc8feba9b7",
    "description": "Deletes the specified SSH public key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SSH Public Key",
      "item": [
        {
          "id": "6269df2b-78dd-4d34-a3ec-2c8760e2a989",
          "name": "deleteSSHPublicKey",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSSHPublicKey?SSHPublicKeyId=SSHPublicKeyId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified SSH public key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ddeb5d2-5c10-4ccb-b378-c99a53871523"
            }
          ]
        }
      ]
    }
  ]
}