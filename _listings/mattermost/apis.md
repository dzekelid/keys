---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Keys
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Reference - Upload private key
  x-api-slug: samlcertificateprivate-post
  description: |-
    Upload the private key to be used for encryption with your SAML configuration. This will also set the filename for the PrivateKeyFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/mattermost/samlcertificateprivate-post-openapi.md
- name: Mattermost API Reference - Remove private key
  x-api-slug: samlcertificateprivate-delete
  description: |-
    Delete the current private key being used with your SAML configuration. This will also disable encryption for SAML on your system as this key is required for that.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/mattermost/samlcertificateprivate-delete-openapi.md
- name: Mattermost API Reference - Remove private key
  x-api-slug: samlcertificateprivate-delete
  description: |-
    Delete the current private key being used with your SAML configuration. This will also disable encryption for SAML on your system as this key is required for that.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/mattermost/samlcertificateprivate-delete-openapi.md
- name: Mattermost API Reference - Upload private key
  x-api-slug: samlcertificateprivate-post
  description: |-
    Upload the private key to be used for encryption with your SAML configuration. This will also set the filename for the PrivateKeyFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/mattermost/samlcertificateprivate-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://matrix.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mattermost.stack.network
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---