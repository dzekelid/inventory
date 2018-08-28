swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Inventory/{partnerId}/Resend:
    put:
      summary: Resend all inventory items.
      description: Request rate limited to 1 request every 5 minutes with bursts up
        to 2 requests.
      operationId: Inventory_ResendAll
      x-api-path-slug: apiv1inventorypartneridresend-put
      parameters:
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Resend
      - ""
      - Inventory
      - Items
  /api/v1/Inventory/Broadcast:
    post:
      summary: Import inventory from CSV.
      description: Request rate limited to 1 request every 60 seconds with bursts
        up to 2 requests.
      operationId: Inventory_Broadcast
      x-api-path-slug: apiv1inventorybroadcast-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Import
      - Inventory
      - From
      - CSV
  /api/v1/Inventory/{partnerId}:
    delete:
      summary: Delete all inventory records.
      description: Request rate limited to 1 request every 60 seconds with bursts
        up to 2 requests.
      operationId: Inventory_DeleteAll
      x-api-path-slug: apiv1inventorypartnerid-delete
      parameters:
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Inventory
      - Records
    post:
      summary: Import inventory from CSV.
      description: Request rate limited to 1 request per second with bursts up to
        2 requests.
      operationId: Inventory_Upload
      x-api-path-slug: apiv1inventorypartnerid-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: path
        name: partnerId
        description: Partner account number
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Import
      - Inventory
      - From
      - CSV
    get:
      summary: Download inventory as CSV.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Inventory_Download
      x-api-path-slug: apiv1inventorypartnerid-get
      parameters:
      - in: query
        name: fileType
        description: CSV or XLSX
      - in: query
        name: includeNullQuantity
        description: Set to true to include items with null quantity
      - in: query
        name: mapped
        description: Set to false to view items with no merchant SKU
      - in: query
        name: modifiedAfter
        description: Only items modified after this time
      - in: path
        name: partnerId
        description: Partner account number
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Download
      - Inventory
      - As
      - CSV