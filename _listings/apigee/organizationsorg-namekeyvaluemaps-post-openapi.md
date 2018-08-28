---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Post Organizations Name Keyvaluemaps
  description: Creates a KeyValueMap.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key
      description: Returns details for a consumer key for a developer app .
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the Developer Email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    post:
      summary: Post Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key
      description: Revokes a developer app key.
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: developer_email
        description: Mention the Developer Email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    delete:
      summary: Delete Organizations Name Developers Developer Email Apps App Name
        Keys Consumer Key
      description: Deletes a consumer key that belongs to an app.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-delete
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the Developer Email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/apiproducts/{apiproduct_name}:
    post:
      summary: Post Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Apiproducts Apiproduct Name
      description: Revokes the association of an API Product with a Developer App's
        consumer key.
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: path
        name: apiproduct_name
        description: Mention the API Product name
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the app name
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - API
      - Products
      - API
      - Productss
    delete:
      summary: Delete Organizations Name Developers Developer Email Apps App Name
        Keys Consumer Key Apiproducts Apiproduct Name
      description: Removes an API product from a developer app key profile, and thereby
        renders the developer app unable to access the URIs defined in the API product
        specified.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductNam
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-delete
      parameters:
      - in: path
        name: apiproduct_name
        description: Mention the API Product name
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the app name
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - API
      - Products
      - API
      - Productss
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth1accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Oauth1accesstokens
      description: Get count of OAuth 1.0 access tokens for a developer's app key.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth1accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth1accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - Oauth1accesstokens
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth2accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Oauth2accesstokens
      description: Get count of OAuth 2.0 access tokens for a developer's app key.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth2accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth2accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the developer name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - Oauth2accesstokens
  /organizations/{org_name}/companies/{company_name}/apps/{app_name}/keys/{consumer_key}:
    get:
      summary: Get Organizations Name Companies Company Name Apps App Name Keys Consumer
        Key
      description: Gets the consumer key issued to a company app.
      operationId: getOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    post:
      summary: Post Organizations Name Companies Company Name Apps App Name Keys Consumer
        Key
      description: Revokes the specific key of a company app.
      operationId: postOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    delete:
      summary: Delete Organizations Name Companies Company Name Apps App Name Keys
        Consumer Key
      description: Deletes a company app key.
      operationId: deleteOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-delete
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
  /organizations/{org_name}/keyvaluemaps:
    get:
      summary: Get Organizations Name Keyvaluemaps
      description: Returns an expanded view of all Maps scoped by organization, environment
        or API.
      operationId: getOrganizationsOrgNameKeyvaluemaps
      x-api-path-slug: organizationsorg-namekeyvaluemaps-get
      parameters:
      - in: query
        name: expand
        description: Set expand value to true
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
    post:
      summary: Post Organizations Name Keyvaluemaps
      description: Creates a KeyValueMap.
      operationId: postOrganizationsOrgNameKeyvaluemaps
      x-api-path-slug: organizationsorg-namekeyvaluemaps-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
  /organizations/{org_name}/keyvaluemaps/{map_name}/entries/{entry_name}:
    get:
      summary: Get Organizations Name Keyvaluemaps Map Name Entries Entry Name
      description: Gets a specific entry details.
      operationId: getOrganizationsOrgNameKeyvaluemapsMapNameEntriesEntryName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-get
      parameters:
      - in: path
        name: entry_name
        description: Mention the entry name
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
      - Entries
      - Entry
    delete:
      summary: Delete Organizations Name Keyvaluemaps Map Name Entries Entry Name
      description: Deletes a single entry by name.
      operationId: deleteOrganizationsOrgNameKeyvaluemapsMapNameEntriesEntryName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-delete
      parameters:
      - in: path
        name: entry_name
        description: Mention the entry name
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
      - Entries
      - Entry
  /organizations/{org_name}/keyvaluemaps/{map_name}:
    get:
      summary: Get Organizations Name Keyvaluemaps Map Name
      description: Gets a KeyValueMap by name, along with associated entries.
      operationId: getOrganizationsOrgNameKeyvaluemapsMapName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-name-get
      parameters:
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
    put:
      summary: Put Organizations Name Keyvaluemaps Map Name
      description: Updates an existing KeyValueMap.
      operationId: putOrganizationsOrgNameKeyvaluemapsMapName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-name-put
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
    delete:
      summary: Delete Organizations Name Keyvaluemaps Map Name
      description: Deletes a KeyValueMap and all associated entries.
      operationId: deleteOrganizationsOrgNameKeyvaluemapsMapName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-name-delete
      parameters:
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---