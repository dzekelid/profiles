---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Retrieves a service profile
  description: "Retrieves the service portfolios of a supplier.   \nA supplier may
    provide more than one type of service. The service profile may be comprised of
    various service portfolios for different service types.  \n- If the login user
    is not an organization admin, he or she can retrieve only the active service portfolios.
    \ \n- if the login user is an organization admin, he or she can retrieve both
    active and inactive service portfolios."
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /masterData:
    get:
      summary: Retrieves supplier profile master data
      description: |-
        Retrieves master data such as processes and materials.
        Narrow down the result by specifying the master data types.
      operationId: retrieves-master-data-such-as-processes-and-materialsnarrow-down-the-result-by-specifying-the-master
      x-api-path-slug: masterdata-get
      parameters:
      - in: query
        name: type
        description: 'A master data typeValid values: [certificates, currencies, materialRequirement,
          postProcesses, preferredLanguages, processMaterial, servicePortfolio]'
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Supplier
      - Profile
      - Master
      - Data
  /organizations/{organizationId}:
    put:
      summary: Updates a supplier profile
      description: |-
        Updates the supplier profile of a specific organization.
        The login user must be from a supplier.
      operationId: updates-the-supplier-profile-of-a-specific-organizationthe-login-user-must-be-from-a-supplier
      x-api-path-slug: organizationsorganizationid-put
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      - in: body
        name: OrganizationUpdateRequest
        description: A request about updating an organization
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Supplier
      - Profile
  /organizations/{organizationId}/serviceProfiles:
    get:
      summary: Retrieves a service profile
      description: "Retrieves the service portfolios of a supplier.   \nA supplier
        may provide more than one type of service. The service profile may be comprised
        of various service portfolios for different service types.  \n- If the login
        user is not an organization admin, he or she can retrieve only the active
        service portfolios.  \n- if the login user is an organization admin, he or
        she can retrieve both active and inactive service portfolios."
      operationId: retrieves-the-service-portfolios-of-a-supplier---a-supplier-may-provide-more-than-one-type-of-servic
      x-api-path-slug: organizationsorganizationidserviceprofiles-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Service
      - Profile
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