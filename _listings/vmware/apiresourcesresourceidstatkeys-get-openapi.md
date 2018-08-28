---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Get StatKeys for Resource and Load var
  description: |-
    Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
    Populates two env vars:
    cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
    cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/resources/{resourceId}/statkeys:
    get:
      summary: Get StatKeys for Resource and Load var
      description: |-
        Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
        Populates two env vars:
        cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
        cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
      operationId: ApiResourcesStatkeysByResourceIdGet2
      x-api-path-slug: apiresourcesresourceidstatkeys-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Statkeys
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