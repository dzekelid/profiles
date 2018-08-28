---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Update Profile Filter
  description: Update an existing profile filter link.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks:
    get:
      summary: Get Profile Filter
      description: Lists all profile filter links for a profile.
      operationId: analytics.management.profileFilterLinks.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinks-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve profile filter links for
      - in: query
        name: max-results
        description: The maximum number of profile filter links to include in this
          response
      - in: path
        name: profileId
        description: Profile ID to retrieve filter links for
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      - in: path
        name: webPropertyId
        description: Web property Id for profile filter links for
      responses:
        200:
          description: OK
      tags:
      - Profile Filter
    post:
      summary: Create Profile Filter
      description: Create a new profile filter link.
      operationId: analytics.management.profileFilterLinks.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinks-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create profile filter link for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: Profile ID to create filter link for
      - in: path
        name: webPropertyId
        description: Web property Id to create profile filter link for
      responses:
        200:
          description: OK
      tags:
      - Profile Filter
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/profileFilterLinks/{linkId}:
    delete:
      summary: Delete Profile Filter
      description: Delete a profile filter link.
      operationId: analytics.management.profileFilterLinks.delete
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to which the profile filter link belongs
      - in: path
        name: linkId
        description: ID of the profile filter link to delete
      - in: path
        name: profileId
        description: Profile ID to which the filter link belongs
      - in: path
        name: webPropertyId
        description: Web property Id to which the profile filter link belongs
      responses:
        200:
          description: OK
      tags:
      - Profile Filter
    get:
      summary: Get Profile Filter
      description: Returns a single profile filter link.
      operationId: analytics.management.profileFilterLinks.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve profile filter link for
      - in: path
        name: linkId
        description: ID of the profile filter link
      - in: path
        name: profileId
        description: Profile ID to retrieve filter link for
      - in: path
        name: webPropertyId
        description: Web property Id to retrieve profile filter link for
      responses:
        200:
          description: OK
      tags:
      - Profile Filter
    patch:
      summary: Update Profile Filter
      description: Update an existing profile filter link. This method supports patch
        semantics.
      operationId: analytics.management.profileFilterLinks.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID to which profile filter link belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: linkId
        description: ID of the profile filter link to be updated
      - in: path
        name: profileId
        description: Profile ID to which filter link belongs
      - in: path
        name: webPropertyId
        description: Web property Id to which profile filter link belongs
      responses:
        200:
          description: OK
      tags:
      - Profile Filter
    put:
      summary: Update Profile Filter
      description: Update an existing profile filter link.
      operationId: analytics.management.profileFilterLinks.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidprofilefilterlinkslinkid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID to which profile filter link belongs
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: linkId
        description: ID of the profile filter link to be updated
      - in: path
        name: profileId
        description: Profile ID to which filter link belongs
      - in: path
        name: webPropertyId
        description: Web property Id to which profile filter link belongs
      responses:
        200:
          description: OK
      tags:
      - Profile Filter
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