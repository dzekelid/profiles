---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Update Profile Background Image
  description: updates user's profile background image
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/update_profile:
    post:
      summary: Update Profile
      description: sets values that users ar eable to set under Account tab
      operationId: sets-values-that-users-ar-eable-to-set-under-account-tab
      x-api-path-slug: accountupdate-profile-post
      parameters:
      - in: query
        name: description
        description: a description of user owning account
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: location
        description: city or country describing where user of account is
      - in: query
        name: name
        description: full name of profile
      - in: query
        name: skip_status
        description: whether or not to include statuses in response
      - in: query
        name: url
        description: url associated with profile
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile_background_image:
    post:
      summary: Update Profile Background Image
      description: updates user's profile background image
      operationId: updates-users-profile-background-image
      x-api-path-slug: accountupdate-profile-background-image-post
      parameters:
      - in: formData
        name: file
        description: image to replace background image of profile
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: skip_status
        description: whether or not to include status in returned user objects
      - in: query
        name: tile
        description: whether or not to tile background image
      - in: query
        name: use
        description: display background image or not
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
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