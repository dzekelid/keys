---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 0
info:
  title: LinkedIn Get Companies Updates Key Update Key
  description: Get companies  updates key update key
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/{id}/updates/key={update-key}/update-comments-as-company/:
    post:
      summary: Add Companies Updates Key Update Key Update Comments As Company
      description: Post companies  updates key update key update comments as company
      operationId: postCompaniesUpdatesKeyUpdateKeyUpdateCommentsAsCompany
      x-api-path-slug: companiesidupdateskeyupdatekeyupdatecommentsascompany-post
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Updates
      - Key
      - Update
      - Key
      - Update
      - Comments
      - As
      - Company
  /companies/{id}/updates/key={update-key}:
    get:
      summary: Get Companies Updates Key Update Key
      description: Get companies  updates key update key
      operationId: getCompaniesUpdatesKeyUpdateKey
      x-api-path-slug: companiesidupdateskeyupdatekey-get
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Updates
      - Key
      - Update
      - Key
  /companies/{id}/updates/key={update-key}/update-comments:
    get:
      summary: Get Companies Updates Key Update Key Update Comments
      description: Get companies  updates key update key update comments
      operationId: getCompaniesUpdatesKeyUpdateKeyUpdateComments
      x-api-path-slug: companiesidupdateskeyupdatekeyupdatecomments-get
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Updates
      - Key
      - Update
      - Key
      - Update
      - Comments
  /companies/{id}/updates/key={update-key}/likes:
    get:
      summary: Get Companies Updates Key Update Key Likes
      description: Get companies  updates key update key likes
      operationId: getCompaniesUpdatesKeyUpdateKeyLikes
      x-api-path-slug: companiesidupdateskeyupdatekeylikes-get
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Updates
      - Key
      - Update
      - Key
      - Likes
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