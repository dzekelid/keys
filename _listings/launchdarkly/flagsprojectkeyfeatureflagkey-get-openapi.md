---
swagger: "2.0"
x-collection-name: LaunchDarkly
x-complete: 0
info:
  title: Launch Darkly Get a single feature flag by key.
  description: Get a single feature flag by key..
  termsOfService: https://launchdarkly.com/terms
  contact:
    name: LaunchDarkly Support
    url: https://support.launchdarkly.com
    email: support@launchdarkly.com
  version: 2.0.0
host: app.launchdarkly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /environments/{projectKey}:
    post:
      summary: Create an environment
      description: Create an environment.
      operationId: postEnvironment
      x-api-path-slug: environmentsprojectkey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Projects
      - Keys
  /environments/{projectKey}/{environmentKey}:
    delete:
      summary: Delete an environment by ID
      description: Delete an environment by id.
      operationId: deleteEnvironment
      x-api-path-slug: environmentsprojectkeyenvironmentkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Projects
      - Keys
      - EnvironmentKey
    get:
      summary: Get an environment by key.
      description: Get an environment by key..
      operationId: getEnvironment
      x-api-path-slug: environmentsprojectkeyenvironmentkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Projects
      - Keys
      - EnvironmentKey
    patch:
      summary: Modify an environment by ID
      description: Modify an environment by id.
      operationId: patchEnvironment
      x-api-path-slug: environmentsprojectkeyenvironmentkey-patch
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Projects
      - Keys
      - EnvironmentKey
  /flag-statuses/{projectKey}/{environmentKey}:
    get:
      summary: Get a list of statuses for all feature flags
      description: Get a list of statuses for all feature flags.
      operationId: getFeatureFlagStatus
      x-api-path-slug: flagstatusesprojectkeyenvironmentkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flag-statuses
      - Projects
      - Keys
      - EnvironmentKey
  /flag-statuses/{projectKey}/{environmentKey}/{featureFlagKey}:
    get:
      summary: Get a list of statuses for all feature flags
      description: Get a list of statuses for all feature flags.
      operationId: getFeatureFlagStatuses
      x-api-path-slug: flagstatusesprojectkeyenvironmentkeyfeatureflagkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flag-statuses
      - Projects
      - Keys
      - EnvironmentKey
      - FeatureFlagKey
  /flags/{projectKey}:
    get:
      summary: Get a list of all features in the given project.
      description: Get a list of all features in the given project..
      operationId: getFeatureFlags
      x-api-path-slug: flagsprojectkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flags
      - Projects
      - Keys
    post:
      summary: Create a feature flag
      description: Create a feature flag.
      operationId: postFeatureFlag
      x-api-path-slug: flagsprojectkey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flags
      - Projects
      - Keys
  /flags/{projectKey}/{featureFlagKey}:
    delete:
      summary: Delete a feature flag by ID
      description: Delete a feature flag by id.
      operationId: deleteFeatureFlag
      x-api-path-slug: flagsprojectkeyfeatureflagkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flags
      - Projects
      - Keys
      - FeatureFlagKey
    get:
      summary: Get a single feature flag by key.
      description: Get a single feature flag by key..
      operationId: getFeatureFlag
      x-api-path-slug: flagsprojectkeyfeatureflagkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flags
      - Projects
      - Keys
      - FeatureFlagKey
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