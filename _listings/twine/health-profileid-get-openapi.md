---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Get a health profile
  description: Get a health profile by id
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /health_profile:
    get:
      summary: List health profiles
      description: Get a list of health profiles
      operationId: fetchHealthProfiles
      x-api-path-slug: health-profile-get
      parameters:
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch health profile
      - in: query
        name: include
        description: List of related resources to include in the response
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Health
      - Profiles
  /health_profile/{id}:
    get:
      summary: Get a health profile
      description: Get a health profile by id
      operationId: fetchHealthProfile
      x-api-path-slug: health-profileid-get
      parameters:
      - in: path
        name: id
        description: Health profile identifier
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Profile
  /health_profile_answer:
    get:
      summary: List health profile answers
      description: Get a list of health profile answers
      operationId: fetchHealthProfileAnswers
      x-api-path-slug: health-profile-answer-get
      parameters:
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch healt profile answers
      - in: query
        name: include
        description: List of related resources to include in the response
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Health
      - Profile
      - Answers
  /health_profile_answer/{id}:
    get:
      summary: Get a health profile answer
      description: Get a health profile answer by id
      operationId: fetchHealthProfileAnswer
      x-api-path-slug: health-profile-answerid-get
      parameters:
      - in: path
        name: id
        description: Health profile answer identifier
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Profile
      - Answer
  /health_profile_question/{id}:
    get:
      summary: Get a health profile question
      description: Get a health profile by id
      operationId: fetchHealthProfileQuestion
      x-api-path-slug: health-profile-questionid-get
      parameters:
      - in: path
        name: id
        description: Health profile question identifier
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Health
      - Profile
      - Question
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