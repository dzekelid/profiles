---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Admin API Profiles Retrieval
  description: Retrieves all available profiles. By default only retrieves ACTILITY-owned
    profiles.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /admin/v140/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /profiles:
    get:
      summary: Profiles Retrieval
      description: Retrieves all available profiles. By default only retrieves ACTILITY-owned
        profiles.
      operationId: retrieves-all-available-profiles-by-default-only-retrieves-actilityowned-profiles
      x-api-path-slug: profiles-get
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Retrieval
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