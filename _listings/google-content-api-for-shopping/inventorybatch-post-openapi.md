---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 0
info:
  title: Google Content API for Shopping API Inventory
  description: Updates price and availability for multiple products or stores in a
    single request. This operation does not update the expiration date of the products.
    This method can only be called for non-multi-client accounts.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /inventory/batch:
    post:
      summary: Inventory
      description: Updates price and availability for multiple products or stores
        in a single request. This operation does not update the expiration date of
        the products. This method can only be called for non-multi-client accounts.
      operationId: content.inventory.custombatch
      x-api-path-slug: inventorybatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Inventory
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