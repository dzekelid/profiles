---
swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 0
info:
  title: My Space Get Profilecomments Personid Self
  description: Retrieves profile comments.
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