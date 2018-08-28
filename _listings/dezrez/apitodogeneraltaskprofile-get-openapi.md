---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get the profile infos for a task
  version: 1.0.0
  description: Get the profile infos for a task.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/general/taskprofile:
    get:
      summary: Get the profile infos for a task
      description: Get the profile infos for a task.
      operationId: GeneralToDo_GetTaskProfileBytaskId
      x-api-path-slug: apitodogeneraltaskprofile-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Infosa
      - Task
  /api/todo/group/taskprofile:
    get:
      summary: Get the profile infos for a task
      description: Get the profile infos for a task.
      operationId: GroupToDo_GetTaskProfileBytaskId
      x-api-path-slug: apitodogrouptaskprofile-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Infosa
      - Task
  /api/todo/property/taskprofile:
    get:
      summary: Get the profile infos for a propery task
      description: Get the profile infos for a propery task.
      operationId: PropertyToDo_GetTaskProfileBytaskId
      x-api-path-slug: apitodopropertytaskprofile-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Infosa
      - Propery
      - Task
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