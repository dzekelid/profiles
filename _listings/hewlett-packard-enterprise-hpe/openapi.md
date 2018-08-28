swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
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
  /virtual-machine-profiles/{id}:
    get:
      summary: Get Virtual Machine Profiles
      description: Returns a virtual machine profile based on its id. It equires any
        project role or non-'consumer' global role.
      operationId: GetVirtualMachineProfileById
      x-api-path-slug: virtualmachineprofilesid-get
      parameters:
      - in: path
        name: id
        description: ID of virtual machine profile to fetch
      responses:
        200:
          description: OK
      tags:
      - Virtual
      - Machine
      - Profiles
  /zone-types/{id}/resource-profiles:
    get:
      summary: Get Zone Types Resource Profiles
      description: Returns all available resourceProfile for **vcenter zone type**.
        It requires the **administrator** role.
      operationId: FindResourceProfileName
      x-api-path-slug: zonetypesidresourceprofiles-get
      parameters:
      - in: path
        name: id
        description: ID of zone-type to fetch
      responses:
        200:
          description: OK
      tags:
      - Zone
      - Types
      - Resource
      - Profiles