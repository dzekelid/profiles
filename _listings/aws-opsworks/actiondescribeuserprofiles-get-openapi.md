---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Describe User Profiles
  version: 1.0.0
  description: Describe specified users.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeUserProfiles:
    get:
      summary: Describe User Profiles
      description: Describe specified users.
      operationId: describeUserProfiles
      x-api-path-slug: actiondescribeuserprofiles-get
      parameters:
      - in: query
        name: IamUserArns
        description: An array of IAM or federated user ARNs that identify the users
          to be described
        type: string
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
        200:
          description: OK
      tags:
      - Describe
      - User
      - Profiles
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