---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get user's profile image
  description: |-
    Get a user's profile image based on user_id string parameter.
    ##### Permissions
    Must be logged in.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/image:
    get:
      summary: Get user's profile image
      description: |-
        Get a user's profile image based on user_id string parameter.
        ##### Permissions
        Must be logged in.
      operationId: get-a-users-profile-image-based-on-user-id-string-parameter-permissionsmust-be-logged-in
      x-api-path-slug: usersuser-idimage-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Profile
      - Image
    post:
      summary: Set user's profile image
      description: |-
        Set a user's profile image based on user_id string parameter.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: set-a-users-profile-image-based-on-user-id-string-parameter-permissionsmust-be-logged-in-as-the-user
      x-api-path-slug: usersuser-idimage-post
      parameters:
      - in: formData
        name: image
        description: The image to be uploaded
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Set
      - Users
      - Profile
      - Image
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