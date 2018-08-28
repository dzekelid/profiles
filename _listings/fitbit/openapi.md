swagger: "2.0"
x-collection-name: Fitbit
x-complete: 1
info:
  title: Fitbit
  description: bring-fitbit-health-data-into-your-apps-including-user-activities-sleep-heart-glucose-and-blood-pressure-information-
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/-/profile.json:
    post:
      summary: Post User Profile.json
      description: Update user's profile using units in the unit system that corresponds
        to the Accept-Language header provided and get a response in the format requested.
      operationId: postUserProfile.json
      x-api-path-slug: userprofile-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Profile.json
  /user/{user-id}/profile.json:
    get:
      summary: Get User User Profile.json
      description: Get user's profile in the format requested using units in the unit
        system which corresponds to the Accept-Language header provided.
      operationId: getUserUserProfile.json
      x-api-path-slug: useruseridprofile-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Profile.json