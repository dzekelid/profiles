swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}:
    get:
      summary: Get user profile
      description: Get profile a user
      operationId: users.id.get
      x-api-path-slug: usersid-get
      parameters:
      - in: path
        name: id
        description: Id of user
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - User
      - Profile