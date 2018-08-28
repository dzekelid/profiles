---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API Base station profiles retrieval
  description: Retrieves the list of existing base station profiles.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /profiles:
    get:
      summary: Profiles Retrieval
      description: Retrieves all available profiles. By default only retrieves ACTILITY-owned
        profiles.
      operationId: retrieves-all-available-profiles-by-default-only-retrieves-actilityowned-profiles
      x-api-path-slug: profiles-get
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Retrieval
  /profiles/{profileId}:
    get:
      summary: Profile Retrieval
      description: Retrieves the profile corresponding to the provided profile Id.
      operationId: retrieves-the-profile-corresponding-to-the-provided-profile-id
      x-api-path-slug: profilesprofileid-get
      parameters:
      - in: path
        name: profileId
        description: Id of the profile to retrieve
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Retrieval
  /deviceProfiles:
    get:
      summary: Device profiles retrieval
      description: Retrieves the list of existing device profiles.
      operationId: retrieves-the-list-of-existing-device-profiles
      x-api-path-slug: deviceprofiles-get
      responses:
        200:
          description: OK
      tags:
      - Device
      - Profiles
      - Retrieval
  /routingProfiles:
    get:
      summary: Routing profiles retrieval
      description: Retrieves a list of existing routing profiles within authorized
        scopes.
      operationId: retrieves-a-list-of-existing-routing-profiles-within-authorized-scopes
      x-api-path-slug: routingprofiles-get
      parameters:
      - in: query
        name: routingProfileId
        description: Id of the routing profile to search for
      responses:
        200:
          description: OK
      tags:
      - Routing
      - Profiles
      - Retrieval
    post:
      summary: Routing profiles creation
      description: Creates a new routing profile.
      operationId: creates-a-new-routing-profile
      x-api-path-slug: routingprofiles-post
      parameters:
      - in: body
        name: routingProfile
        description: Contents of the routing profile to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Routing
      - Profiles
      - Creation
  /baseStationProfiles:
    get:
      summary: Base station profiles retrieval
      description: Retrieves the list of existing base station profiles.
      operationId: retrieves-the-list-of-existing-base-station-profiles
      x-api-path-slug: basestationprofiles-get
      responses:
        200:
          description: OK
      tags:
      - Base
      - Station
      - Profiles
      - Retrieval
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