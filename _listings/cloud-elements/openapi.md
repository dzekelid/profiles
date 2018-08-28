swagger: "2.0"
x-collection-name: Cloud Elements
x-complete: 1
info:
  title: zohocrm
  version: api-v2
host: console.cloud-elements.com
basePath: /elements/api-v2/hubs/crm
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