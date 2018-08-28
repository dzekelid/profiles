swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/profile:
    get:
      summary: Get user profile
      description: Get user profile.
      operationId: get-user-profile
      x-api-path-slug: usersuser-idprofile-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Profile