{
  "info": {
    "name": "AWS Identity and Access Management API Get S S H Public Key",
    "_postman_id": "55a97eec-5774-425b-acc0-10bc54b39296",
    "description": "Retrieves the specified SSH public key, including metadata about the key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SSH Public Key",
      "item": [
        {
          "id": "10d4726d-feed-4b0d-97a8-bf4d66edbcf5",
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
              "id": "85409121-37a9-4133-8712-1ee4e6b680e9"
            }
          ]
        },
        {
          "id": "e8d6bcb7-4ca1-4e71-a2ac-1f9da3ba46ae",
          "name": "getSSHPublicKey",
          "request": {
            "url": "http://example.com/api/?Action=GetSSHPublicKey?Encoding=Encoding&SSHPublicKeyId=SSHPublicKeyId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified SSH public key, including metadata about the key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23bf7f0d-697c-45c0-a852-21f485e72df9"
            }
          ]
        }
      ]
    }
  ]
}