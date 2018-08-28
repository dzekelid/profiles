---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Profile
  description: Mobile API User Profile
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/user/profile:
    get:
      summary: Profile
      description: Mobile API User Profile
      operationId: profile-user
      x-api-path-slug: apiuserprofile-get
      parameters:
      - in: query
        name: profileTypes
        description: This is a comma-separated list of profile types to retrieve when
          the login is processed
      - in: query
        name: retrieveCoupons
        description: Whether to include user coupons in the response
      - in: query
        name: tuid
        description: The tuid of the user/account whose profile you would like
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Users
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