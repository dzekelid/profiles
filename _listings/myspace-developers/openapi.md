swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 1
info:
  title: My Space
  description: create-apps-and-games-within-the-myspace-platform--monetize-through-advertising-and-virtual-goods-
  version: 1.0.0
host: api.myspace.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1.0/profilecomments/{personId}/@self:
    get:
      summary: Get Profilecomments Personid Self
      description: Retrieves profile comments.
      operationId: 1.0.profilecomments.personId._self.get
      x-api-path-slug: 1-0profilecommentspersonidself-get
      parameters:
      - in: path
        name: personId
        description: The persons identifier
      responses:
        200:
          description: OK
      tags:
      - Profilecomments
      - People
      - Self