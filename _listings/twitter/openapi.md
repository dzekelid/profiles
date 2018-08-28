swagger: "2.0"
x-collection-name: Twitter
x-complete: 1
info:
  title: Twitter
  description: the-twitter-api-gives-you-programmatic-control-over-any-twitter-account-and-most-aspect-of-the-platform--allowing-developers-to-build-social-applications-that-use-the-platform-and-automate-interactions-between-users-
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/update_profile:
    post:
      summary: Update Profile
      description: sets values that users ar eable to set under Account tab
      operationId: sets-values-that-users-ar-eable-to-set-under-account-tab
      x-api-path-slug: accountupdate-profile-post
      parameters:
      - in: query
        name: description
        description: a description of user owning account
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: location
        description: city or country describing where user of account is
      - in: query
        name: name
        description: full name of profile
      - in: query
        name: skip_status
        description: whether or not to include statuses in response
      - in: query
        name: url
        description: url associated with profile
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile_background_image:
    post:
      summary: Update Profile Background Image
      description: updates user's profile background image
      operationId: updates-users-profile-background-image
      x-api-path-slug: accountupdate-profile-background-image-post
      parameters:
      - in: formData
        name: file
        description: image to replace background image of profile
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: skip_status
        description: whether or not to include status in returned user objects
      - in: query
        name: tile
        description: whether or not to tile background image
      - in: query
        name: use
        description: display background image or not
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile_colors:
    post:
      summary: Update Profile Colors
      description: sets one or more hex values that controls color scheme
      operationId: sets-one-or-more-hex-values-that-controls-color-scheme
      x-api-path-slug: accountupdate-profile-colors-post
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: profile_background_color
        description: profile background color
      - in: query
        name: profile_link_color
        description: profile link color
      - in: query
        name: profile_sidebar_border_color
        description: profile sidebars border color
      - in: query
        name: profile_sidebar_fill_color
        description: profiles sidebar background color
      - in: query
        name: profile_text_color
        description: profile text color
      - in: query
        name: skip_status
        description: whether or not to include statuses
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile_image:
    post:
      summary: Update Profile Image
      description: updates user's profile image
      operationId: updates-users-profile-image
      x-api-path-slug: accountupdate-profile-image-post
      parameters:
      - in: formData
        name: image
        description: image to be set as profile image
      - in: query
        name: skip_status
        description: whether or not to include statuses
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account