swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
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
        200:
          description: OK
      tags:
      - Describe
      - User
      - Profiles
  /?Action=CreateUserProfile:
    get:
      summary: Create User Profile
      description: Creates a new user profile.
      operationId: createUserProfile
      x-api-path-slug: actioncreateuserprofile-get
      parameters:
      - in: query
        name: AllowSelfManagement
        description: Whether users can specify their own SSH public key through the
          My Settings page
        type: string
      - in: query
        name: IamUserArn
        description: The users IAM ARN; this can also be a federated users ARN
        type: string
      - in: query
        name: SshPublicKey
        description: The users public SSH key
        type: string
      - in: query
        name: SshUsername
        description: The users SSH user name
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Profile
  /?Action=DeleteUserProfile:
    get:
      summary: Delete User Profile
      description: Deletes a user profile.
      operationId: deleteUserProfile
      x-api-path-slug: actiondeleteuserprofile-get
      parameters:
      - in: query
        name: IamUserArn
        description: The users IAM ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Profile
  /?Action=DescribeMyUserProfile:
    get:
      summary: Describe My User Profile
      description: Describes a user's SSH information.
      operationId: describeMyUserProfile
      x-api-path-slug: actiondescribemyuserprofile-get
      parameters:
      - in: query
        name: UserProfile
        description: A UserProfile object that describes the users SSH information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - My
      - User
      - Profile
  /?Action=UpdateMyUserProfile:
    get:
      summary: Update My User Profile
      description: Updates a user's SSH public key.
      operationId: updateMyUserProfile
      x-api-path-slug: actionupdatemyuserprofile-get
      parameters:
      - in: query
        name: SshPublicKey
        description: The users SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - My
      - User
      - Profile
  /?Action=UpdateUserProfile:
    get:
      summary: Update User Profile
      description: Updates a specified user profile.
      operationId: updateUserProfile
      x-api-path-slug: actionupdateuserprofile-get
      parameters:
      - in: query
        name: AllowSelfManagement
        description: Whether users can specify their own SSH public key through the
          My Settings page
        type: string
      - in: query
        name: IamUserArn
        description: The user IAM ARN
        type: string
      - in: query
        name: SshPublicKey
        description: The users new SSH public key
        type: string
      - in: query
        name: SshUsername
        description: The users SSH user name
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Profile