---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Sets whether inventory is needed on tenant role
  version: 1.0.0
  description: Sets whether inventory is needed on tenant role.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/progression/lettings/{roleId}/inventory/uploaddocument:
    post:
      summary: Uploads an inventory document for a tenant role
      description: Uploads an inventory document for a tenant role.
      operationId: LettingsProgression_UploadAndAttachInventoryDocumentByroleIdBydocumentSaveCommand
      x-api-path-slug: apiprogressionlettingsroleidinventoryuploaddocument-post
      parameters:
      - in: body
        name: documentSaveCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: Tenant role id
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Inventory
      - Documenta
      - Tenant
      - Role
  /api/progression/lettings/{roleId}/inventory/setrequired:
    post:
      summary: Sets whether inventory is needed on tenant role
      description: Sets whether inventory is needed on tenant role.
      operationId: LettingsProgression_SetInventoryRequiredByroleIdByrequired
      x-api-path-slug: apiprogressionlettingsroleidinventorysetrequired-post
      parameters:
      - in: query
        name: required
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: Tenant Role Id
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Whether
      - Inventory
      - Is
      - Needed
      - "On"
      - Tenant
      - Role
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