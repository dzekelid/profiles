---
swagger: "2.0"
x-collection-name: Flat
x-complete: 0
info:
  title: Flat Get a public user profile
  description: Get a public profile of a Flat User.
  termsOfService: https://flat.io/legal
  contact:
    name: Flat
    url: https://flat.io/support
    email: developers@flat.io
  version: 2.1.0
host: api.flat.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me:
    get:
      summary: Get current user profile
      description: Get details about the current authenticated User.
      operationId: getAuthenticatedUser
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Current
      - User
      - Profile
  /users/{user}:
    get:
      summary: Get a public user profile
      description: Get a public profile of a Flat User.
      operationId: getUser
      x-api-path-slug: usersuser-get
      parameters:
      - in: path
        name: user
        description: This route parameter is the unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Public
      - User
      - Profile
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