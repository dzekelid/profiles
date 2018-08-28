swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /publisher/{accountId}/profiles:
    get:
      summary: Get Publish Profiles
      description: Gets the requested publisher profile(s) by publisher accountId.
      operationId: adexchangebuyer.pubprofiles.list
      x-api-path-slug: publisheraccountidprofiles-get
      parameters:
      - in: path
        name: accountId
        description: The accountId of the publisher to get profiles for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Profile