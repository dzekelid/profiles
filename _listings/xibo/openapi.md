swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displayprofile:
    get:
      summary: Display Profile Search
      description: Search this users Display Profiles
      operationId: displayProfileSearch
      x-api-path-slug: displayprofile-get
      parameters:
      - in: formData
        name: displayProfile
        description: Filter by DisplayProfile Name
      - in: formData
        name: displayProfileId
        description: Filter by DisplayProfile Id
      - in: formData
        name: type
        description: Filter by DisplayProfile Type (windows|android)
      responses:
        200:
          description: OK
      tags:
      - Display
      - Profile
      - Search
    post:
      summary: Add Display Profile
      description: Add a Display Profile
      operationId: displayProfileAdd
      x-api-path-slug: displayprofile-post
      parameters:
      - in: formData
        name: isDefault
        description: Flag indicating if this is the default profile for the client
          type
      - in: formData
        name: name
        description: The Name of the Display Profile
      - in: formData
        name: type
        description: The Client Type this Profile will apply to
      responses:
        200:
          description: OK
      tags:
      - Display
      - Profile
  /displayprofile/{displayProfileId}:
    put:
      summary: Edit Display Profile
      description: Edit a Display Profile
      operationId: displayProfileEdit
      x-api-path-slug: displayprofiledisplayprofileid-put
      parameters:
      - in: path
        name: displayProfileId
        description: The Display Profile ID
      - in: formData
        name: isDefault
        description: Flag indicating if this is the default profile for the client
          type
      - in: formData
        name: name
        description: The Name of the Display Profile
      - in: formData
        name: type
        description: The Client Type this Profile will apply to
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Display
      - Profile
    delete:
      summary: Delete Display Profile
      description: Delete an existing Display Profile
      operationId: displayProfileDelete
      x-api-path-slug: displayprofiledisplayprofileid-delete
      parameters:
      - in: path
        name: displayProfileId
        description: The Display Profile ID
      responses:
        200:
          description: OK
      tags:
      - Display
      - Profile