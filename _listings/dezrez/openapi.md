swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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