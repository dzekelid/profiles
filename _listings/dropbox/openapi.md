swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
basePath: /1
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