---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Create Login Profile
  version: 1.0.0
  description: |-
    Creates a password for the specified user, giving the user the ability to access AWS
          services through the AWS Management Console.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListInstanceProfiles:
    get:
      summary: List Instance Profiles
      description: Lists the instance profiles that have the specified path prefix.
      operationId: listInstanceProfiles
      x-api-path-slug: actionlistinstanceprofiles-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=ListInstanceProfilesForRole:
    get:
      summary: List Instance Profiles For Role
      description: Lists the instance profiles that have the specified associated
        IAM role.
      operationId: listInstanceProfilesForRole
      x-api-path-slug: actionlistinstanceprofilesforrole-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: RoleName
        description: The name of the role to list instance profiles for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles For Role
  /?Action=AddRoleToInstanceProfile:
    get:
      summary: Add Role To Instance Profile
      description: Adds the specified IAM role to the specified instance profile.
      operationId: addRoleToInstanceProfile
      x-api-path-slug: actionaddroletoinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to update
        type: string
      - in: query
        name: RoleName
        description: The name of the role to add
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Instance
  /?Action=CreateInstanceProfile:
    get:
      summary: Create Instance Profile
      description: Creates a new instance profile.
      operationId: createInstanceProfile
      x-api-path-slug: actioncreateinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to create
        type: string
      - in: query
        name: Path
        description: The path to the instance profile
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=CreateLoginProfile:
    get:
      summary: Create Login Profile
      description: |-
        Creates a password for the specified user, giving the user the ability to access AWS
              services through the AWS Management Console.
      operationId: createLoginProfile
      x-api-path-slug: actioncreateloginprofile-get
      parameters:
      - in: query
        name: Password
        description: The new password for the user
        type: string
      - in: query
        name: PasswordResetRequired
        description: Specifies whether the user is required to set a new password
          on next sign-in
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to create a password for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
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