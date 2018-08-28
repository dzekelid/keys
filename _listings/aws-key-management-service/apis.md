---
name: AWS Key Management Service
x-slug: aws-key-management-service
description: AWS Key Management Service (KMS) is a managed service that makes it easy
  for you to create and control the encryption keys used to encrypt your data, and
  uses Hardware Security Modules (HSMs) to protect the security of your keys. AWS
  Key Management Service is integrated with several other AWS services to help you
  protect the data you store with these services. AWS Key Management Service is also
  integrated with AWS CloudTrail to provide you with logs of all key usage to help
  meet your regulatory and compliance needs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Key Management Service API - Cancel Key Deletion
  x-api-slug: actioncancelkeydeletion-get
  description: Cancels the deletion of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actioncancelkeydeletion-get-openapi.md
- name: AWS Key Management Service API - Create Key
  x-api-slug: actioncreatekey-get
  description: Creates a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actioncreatekey-get-openapi.md
- name: AWS Key Management Service API - Delete Imported Key Material
  x-api-slug: actiondeleteimportedkeymaterial-get
  description: |-
    Deletes key material that you previously imported and makes the specified customer
          master key (CMK) unusable.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondeleteimportedkeymaterial-get-openapi.md
- name: AWS Key Management Service API - Describe Key
  x-api-slug: actiondescribekey-get
  description: Provides detailed information about the specified customer master key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondescribekey-get-openapi.md
- name: AWS Key Management Service API - Disable Key
  x-api-slug: actiondisablekey-get
  description: |-
    Sets the state of a customer master key (CMK) to disabled, thereby preventing its use
          for cryptographic operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondisablekey-get-openapi.md
- name: AWS Key Management Service API - Disable Key Rotation
  x-api-slug: actiondisablekeyrotation-get
  description: Disables rotation of the specified key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondisablekeyrotation-get-openapi.md
- name: AWS Key Management Service API - Enable Key
  x-api-slug: actionenablekey-get
  description: Marks a key as enabled, thereby permitting its use.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionenablekey-get-openapi.md
- name: AWS Key Management Service API - Enable Key Rotation
  x-api-slug: actionenablekeyrotation-get
  description: Enables rotation of the specified customer master key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionenablekeyrotation-get-openapi.md
- name: AWS Key Management Service API - Generate Data Key
  x-api-slug: actiongeneratedatakey-get
  description: |-
    Returns a data encryption key that you can use in your application to encrypt
          data locally.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiongeneratedatakey-get-openapi.md
- name: AWS Key Management Service API - Generate Data Key Without Plaintext
  x-api-slug: actiongeneratedatakeywithoutplaintext-get
  description: Returns a data encryption key encrypted under a customer master key
    (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiongeneratedatakeywithoutplaintext-get-openapi.md
- name: AWS Key Management Service API - Get Key Rotation Status
  x-api-slug: actiongetkeyrotationstatus-get
  description: |-
    Retrieves a Boolean value that indicates whether key rotation is enabled for the
          specified key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiongetkeyrotationstatus-get-openapi.md
- name: AWS Key Management Service API - Import Key Material
  x-api-slug: actionimportkeymaterial-get
  description: |-
    Imports key material into an AWS KMS customer master key (CMK) from your existing key
          management infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionimportkeymaterial-get-openapi.md
- name: AWS Key Management Service API - List Keys
  x-api-slug: actionlistkeys-get
  description: Lists the customer master keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionlistkeys-get-openapi.md
- name: AWS Key Management Service API - Put Key Policy
  x-api-slug: actionputkeypolicy-get
  description: Attaches a key policy to the specified customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionputkeypolicy-get-openapi.md
- name: AWS Key Management Service API - Schedule Key Deletion
  x-api-slug: actionschedulekeydeletion-get
  description: Schedules the deletion of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionschedulekeydeletion-get-openapi.md
- name: AWS Key Management Service API - Update Key Description
  x-api-slug: actionupdatekeydescription-get
  description: Updates the description of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionupdatekeydescription-get-openapi.md
- name: AWS Key Management Service API - Cancel Key Deletion
  x-api-slug: actioncancelkeydeletion-get
  description: Cancels the deletion of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actioncancelkeydeletion-get-openapi.md
- name: AWS Key Management Service API - Create Key
  x-api-slug: actioncreatekey-get
  description: Creates a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actioncreatekey-get-openapi.md
- name: AWS Key Management Service API - Delete Imported Key Material
  x-api-slug: actiondeleteimportedkeymaterial-get
  description: |-
    Deletes key material that you previously imported and makes the specified customer
          master key (CMK) unusable.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondeleteimportedkeymaterial-get-openapi.md
- name: AWS Key Management Service API - Describe Key
  x-api-slug: actiondescribekey-get
  description: Provides detailed information about the specified customer master key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondescribekey-get-openapi.md
- name: AWS Key Management Service API - Disable Key
  x-api-slug: actiondisablekey-get
  description: |-
    Sets the state of a customer master key (CMK) to disabled, thereby preventing its use
          for cryptographic operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondisablekey-get-openapi.md
- name: AWS Key Management Service API - Disable Key Rotation
  x-api-slug: actiondisablekeyrotation-get
  description: Disables rotation of the specified key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiondisablekeyrotation-get-openapi.md
- name: AWS Key Management Service API - Enable Key
  x-api-slug: actionenablekey-get
  description: Marks a key as enabled, thereby permitting its use.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionenablekey-get-openapi.md
- name: AWS Key Management Service API - Enable Key Rotation
  x-api-slug: actionenablekeyrotation-get
  description: Enables rotation of the specified customer master key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionenablekeyrotation-get-openapi.md
- name: AWS Key Management Service API - Generate Data Key
  x-api-slug: actiongeneratedatakey-get
  description: |-
    Returns a data encryption key that you can use in your application to encrypt
          data locally.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiongeneratedatakey-get-openapi.md
- name: AWS Key Management Service API - Generate Data Key Without Plaintext
  x-api-slug: actiongeneratedatakeywithoutplaintext-get
  description: Returns a data encryption key encrypted under a customer master key
    (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiongeneratedatakeywithoutplaintext-get-openapi.md
- name: AWS Key Management Service API - Get Key Policy
  x-api-slug: actiongetkeypolicy-get
  description: Retrieves a policy attached to the specified key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiongetkeypolicy-get-openapi.md
- name: AWS Key Management Service API - Get Key Rotation Status
  x-api-slug: actiongetkeyrotationstatus-get
  description: |-
    Retrieves a Boolean value that indicates whether key rotation is enabled for the
          specified key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actiongetkeyrotationstatus-get-openapi.md
- name: AWS Key Management Service API - Import Key Material
  x-api-slug: actionimportkeymaterial-get
  description: |-
    Imports key material into an AWS KMS customer master key (CMK) from your existing key
          management infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionimportkeymaterial-get-openapi.md
- name: AWS Key Management Service API - Import Key Material
  x-api-slug: actionimportkeymaterial-get
  description: |-
    Imports key material into an AWS KMS customer master key (CMK) from your existing key
          management infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionimportkeymaterial-get-openapi.md
- name: AWS Key Management Service API - List Key Policies
  x-api-slug: actionlistkeypolicies-get
  description: Retrieves a list of policies attached to a key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionlistkeypolicies-get-openapi.md
- name: AWS Key Management Service API - List Key Policies
  x-api-slug: actionlistkeypolicies-get
  description: Retrieves a list of policies attached to a key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionlistkeypolicies-get-openapi.md
- name: AWS Key Management Service API - List Keys
  x-api-slug: actionlistkeys-get
  description: Lists the customer master keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionlistkeys-get-openapi.md
- name: AWS Key Management Service API - List Keys
  x-api-slug: actionlistkeys-get
  description: Lists the customer master keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionlistkeys-get-openapi.md
- name: AWS Key Management Service API - Put Key Policy
  x-api-slug: actionputkeypolicy-get
  description: Attaches a key policy to the specified customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionputkeypolicy-get-openapi.md
- name: AWS Key Management Service API - Put Key Policy
  x-api-slug: actionputkeypolicy-get
  description: Attaches a key policy to the specified customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionputkeypolicy-get-openapi.md
- name: AWS Key Management Service API - Schedule Key Deletion
  x-api-slug: actionschedulekeydeletion-get
  description: Schedules the deletion of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionschedulekeydeletion-get-openapi.md
- name: AWS Key Management Service API - Schedule Key Deletion
  x-api-slug: actionschedulekeydeletion-get
  description: Schedules the deletion of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionschedulekeydeletion-get-openapi.md
- name: AWS Key Management Service API - Update Key Description
  x-api-slug: actionupdatekeydescription-get
  description: Updates the description of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionupdatekeydescription-get-openapi.md
- name: AWS Key Management Service API - Update Key Description
  x-api-slug: actionupdatekeydescription-get
  description: Updates the description of a customer master key (CMK).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-key-management.jpg
  humanURL: https://aws.amazon.com/kms/
  baseURL: :///
  tags: Amazon Web Services, Encryption, Security, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/aws-key-management-service/actionupdatekeydescription-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.internet.of.things.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.key.management.service.stack.network
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/kms/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/kms/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/kms/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/kms/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/kms/pricing/
- type: x-website
  url: https://aws.amazon.com/kms/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---