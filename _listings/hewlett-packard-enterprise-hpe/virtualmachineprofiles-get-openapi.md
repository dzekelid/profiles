---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Get Virtual Machine Profiles
  description: Returns all virtual machine profiles. It requires any project role
    or non-'consumer' global role.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /virtual-machine-profiles:
    get:
      summary: Get Virtual Machine Profiles
      description: Returns all virtual machine profiles. It requires any project role
        or non-'consumer' global role.
      operationId: FindVirtualMachineProfiles
      x-api-path-slug: virtualmachineprofiles-get
      parameters:
      - in: query
        name: serviceUri
        description: service to filter virtual machine profiles by
      - in: query
        name: zoneUri
        description: Zone to filter virtual machine profiles by
      responses:
        200:
          description: OK
      tags:
      - Virtual
      - Machine
      - Profiles
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