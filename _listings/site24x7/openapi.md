---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 1
info:
  title: Threshold Profile API
  description: the-threshold-profile-api-
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /threshold_profiles/{profile_id}:
    get:
      summary: Retrieve Threshold Profile
      description: Retrieve the configuration of a Threshold profile.
      operationId: retrieve-threshold-profile
      x-api-path-slug: threshold-profilesprofile-id-get
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
      tags:
      - Threshold Profiles
    delete:
      summary: Delete Threshold Profile
      description: Delete an existing Threshold profile.
      operationId: delete-threshold-profile
      x-api-path-slug: threshold-profilesprofile-id-delete
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
      tags:
      - Threshold Profiles
---