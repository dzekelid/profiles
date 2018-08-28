---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Cloud Elements - Dropbox For Business API Set Profile
  description: Set profile.
  version: "1"
host: api.dropbox.com
basePath: /1/team
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/set_profile:
    get:
      summary: Set Profile
      description: Set profile.
      operationId: getMembersSetProfile
      x-api-path-slug: membersset-profile-get
      parameters:
      - in: query
        name: external_id
        description: optional external ID
      - in: query
        name: member_id
        description: optional member ID
      - in: query
        name: new_email
        description: optional new email for member
      - in: query
        name: new_external_id
        description: optional new external ID for member
      - in: query
        name: new_given_name
        description: optional new given name for member
      - in: query
        name: new_surname
        description: optional new surname for member
      responses:
        200:
          description: OK
      tags:
      - Set
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