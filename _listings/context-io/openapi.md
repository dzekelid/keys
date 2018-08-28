swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth_providers/{key}:
    get:
      summary: Get Oauth Provers Key
      description: Gets information about a given OAuth provider.
      operationId: getOauthProvider_
      x-api-path-slug: oauth-providerskey-get
      parameters:
      - in: path
        name: key
        description: The consumer key for this external OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
      - Key
    delete:
      summary: Delete Oauth Provers Key
      description: Removes a given OAuth provider.
      operationId: removeOauthProvider_
      x-api-path-slug: oauth-providerskey-delete
      parameters:
      - in: path
        name: key
        description: The consumer key for this external OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
      - Key