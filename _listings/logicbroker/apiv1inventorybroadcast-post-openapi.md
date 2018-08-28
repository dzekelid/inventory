---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Import inventory from CSV.
  version: 1.0.0
  description: Request rate limited to 1 request every 60 seconds with bursts up to
    2 requests.
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