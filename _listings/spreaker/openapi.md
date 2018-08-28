swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/image:
    put:
      summary: Change User Profile Image
      description: Change User Profile Image
      operationId: putUserUserImage
      x-api-path-slug: useruser-idimage-put
      parameters:
      - in: query
        name: image_id
        description: The id of the image to set to the user profile
      - in: path
        name: user_id
        description: The unique user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - User
      - Profile
      - Image