---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Photo Comments v2
  description: This method returns comments on meetup photos. To post messages, see
    the corresponding write method
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/:member_id:
    patch:
      summary: Member Profile Edit
      description: Edits Member Profiles.For Group Profiles, see [this endpoint](/meetup_api/docs/:urlname/members/:member_id)
      operationId: profiles
      x-api-path-slug: membersmember-id-patch
      parameters:
      - in: query
        name: add_topics
        description: Comma-delimited list of topic ids to add to members interest
          list
        type: string
      - in: query
        name: bio
        description: Member bio of up to 250 characters
        type: string
      - in: query
        name: bio_privacy
        description: Preference for hiding or showing member bio to others
        type: string
      - in: query
        name: birthday
        description: Members date or year of birth
        type: string
      - in: query
        name: city_id
        description: Valid Meetup city identifier that indicates the city in which
          the member resides
        type: string
      - in: query
        name: facebook_privacy
        description: Preference for hiding showing information members facebook connection
        type: string
      - in: query
        name: gender
        description: Members gender
        type: string
      - in: query
        name: groups_privacy
        description: Preference for hiding or showing group memberships to others
        type: string
      - in: query
        name: lang
        description: Members language preference
        type: string
      - in: query
        name: lat
        description: A valid latitude to resolve the closest location to associate
          with the member
        type: string
      - in: query
        name: lon
        description: A valid longitude to resolve the closest location to associate
          with the memberThis parameter must be accompanied by lat and zip
        type: string
      - in: query
        name: messaging_pref
        description: Preference for which members may contact you via the Meetup platform
        type: string
      - in: query
        name: name
        description: Member name
        type: string
      - in: query
        name: photo_id
        description: A valid photo id to this member has previously updated to use
          as profile photo
        type: string
      - in: query
        name: remove_topics
        description: Comma-delimited list of topic ids to remove from members interest
          list
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all the groupprofile
          photos for the member with the provided photo_id
        type: string
      - in: query
        name: topics_privacy
        description: Preference for hiding or showing member interests to others
        type: string
      - in: query
        name: zip
        description: A valid zip code to associate with the member
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profiles
  /2/profiles:
    get:
      summary: Profiles
      description: This method returns member *profiles* associated with a particular
        group. Meetup members have separate profiles for each group they join.
      operationId: profiles
      x-api-path-slug: 2profiles-get
      parameters:
      - in: query
        name: fields
        description: comma delimited list of optional response properties
        type: string
      - in: query
        name: group_id
        description: Return profiles in the group with this ID
        type: string
      - in: query
        name: group_urlname
        description: Return profiles for the group with the given custom URL path
        type: string
      - in: query
        name: member_id
        description: Return the profiles for members with these IDs, separated by
          commas
        type: string
      - in: query
        name: role
        description: if leads, only profiles for members of the leadership team are
          included
        type: string
      - in: query
        name: status
        description: Status filter for members
        type: string
      - in: query
        name: topic, groupnum
        description: Group identification by topic, deprecated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profile
  /2/profile:
    post:
      summary: Profile Create (Group Join)
      description: This method allows an authenticated member to join a group by creating
        a profile
      operationId: profiles
      x-api-path-slug: 2profile-post
      parameters:
      - in: query
        name: answer_{qid}
        description: Answers to questions from groups API join_info question fields
        type: string
      - in: query
        name: group_id
        description: Id of group to join
        type: string
      - in: query
        name: group_urlname
        description: Urlname of group to join
        type: string
      - in: query
        name: intro
        description: Provides a Member an opportunity to tell the group about themselves
        type: string
      - in: query
        name: new_photo
        description: file upload for a new member photo
        type: string
      - in: query
        name: photo_id
        description: photo_id of the photo to use for this profile
        type: string
      - in: query
        name: site_name
        description: Name of members site
        type: string
      - in: query
        name: site_url
        description: Link to members site
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profile
  /2/profile/:gid/:mid:
    post:
      summary: Profile Edit
      description: Update a member's group profile
      operationId: profiles
      x-api-path-slug: 2profilegidmid-post
      parameters:
      - in: query
        name: add_role
        description: 'Allows those with permission to assign one of the following
          roles: coorganizer, event_organizer, assistant_organizer'
        type: string
      - in: query
        name: answer_{qid}
        description: Answers to questions from groups API join_info question fields
        type: string
      - in: query
        name: intro
        description: Provides a Member an opportunity to tell the group about themselves
        type: string
      - in: query
        name: new_photo
        description: file upload for a new member photo
        type: string
      - in: query
        name: photo_id
        description: photo_id of the photo to use for this profile
        type: string
      - in: query
        name: remove_role
        description: 'Allows those with permission to remove one of the following
          roles: coorganizer, event_organizer, assistant_organizer'
        type: string
      - in: query
        name: site_name
        description: Name of members site
        type: string
      - in: query
        name: site_url
        description: Link to members site
        type: string
      - in: query
        name: title
        description: An organizer-defined member title
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profile
    get:
      summary: Profile Get
      description: Retrieves a single group profile
      operationId: profiles
      x-api-path-slug: 2profilegidmid-get
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profile
    delete:
      summary: Profile Delete (Leave Group)
      description: Deletes a member's group profile
      operationId: profiles
      x-api-path-slug: 2profilegidmid-delete
      parameters:
      - in: query
        name: exit_comment
        description: Optional message to the organizer when leaving
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profile
  /2/photo_comments:
    get:
      summary: Photo Comments v2
      description: This method returns comments on meetup photos. To post messages,
        see the corresponding write method
      operationId: photos
      x-api-path-slug: 2photo-comments-get
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: member_id
        description: Return comments for the given member_ids, separated by commas
        type: string
      - in: query
        name: photo_id
        description: Return comments on these photos, separated by commas
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Profile
  /:urlname/members/:member_id:
    get:
      summary: Get Group Member Profile
      description: |-
        Gets Group Profiles.
        For Member Profiles, see [this endpoint](/meetup_api/docs/members/:member_id)
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    patch:
      summary: Edit Group Member Profile
      description: |-
        Edits Group Profiles.
        To fetch Group Member Profiles,
        see [this endpoint](/meetup_api/docs/:urlname/members/:member_id#get)
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-patch
      parameters:
      - in: query
        name: add_role
        description: Allows those with permission to assign one of the following roles:assistant_organizer,
          coorganizer, or event_organizer
        type: string
      - in: query
        name: answer_{qid}
        description: Answers to questions from groups API join_info question fields
        type: string
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      - in: query
        name: intro
        description: Provides a Member an opportunity to tell the group about themselves,in
          at most 255 characters
        type: string
      - in: query
        name: photo_id
        description: Numeric id of the photo to use for this profile
        type: string
      - in: query
        name: remove_role
        description: Allows those with permission to remove one of the following roles:assistant_organizer,
          coorganizer, or event_organizer
        type: string
      - in: query
        name: title
        description: An organizer-defined title,in at most 255 characters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    delete:
      summary: Delete Group Member Profile (Leave Group)
      description: Deletes a member's group profiles.
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-delete
      parameters:
      - in: query
        name: exit_comment
        description: Optional message to the organizer when leaving
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /:urlname/members:
    get:
      summary: Group Profile list
      description: Get a list of Meetup group members
      operationId: profiles
      x-api-path-slug: urlnamemembers-get
      parameters:
      - in: query
        name: desc
        description: Boolean value controling sort order of results
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: filter
        description: May be set to stepup_eligible to return only members eligible
          to step up as organizer
        type: string
      - in: query
        name: order
        description: Orders results according to definitions listed below
        type: string
      - in: query
        name: page
        description: Number of requested members to return
        type: string
      - in: query
        name: role
        description: May be set to leads to filter returned members on the lead team
        type: string
      - in: query
        name: status
        description: A comma-delimited list of member statuses
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
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