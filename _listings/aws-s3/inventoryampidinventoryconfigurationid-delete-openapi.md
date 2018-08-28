---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 DELETE Bucket inventory configuration
  version: 1.0.0
  description: This implementation of the DELETE operation deletes an inventory configuration(identified
    by the inventory configuration ID) from the bucket
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?inventory:
    get:
      summary: List Bucket Inventory Configurations
      description: This implementation of the GET operation returns a list of inventoryconfigurations
        for the bucket
      operationId: list-bucket-inventory-configurations
      x-api-path-slug: inventory-get
      parameters:
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue an inventory configuration
          listing that has beenttttttttttruncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Inventory
      - Configurations
  /?inventory&amp;id=configuration-ID:
    put:
      summary: PUT Bucket inventory configuration
      description: This implementation of the PUT operation adds an inventory configuration(identified
        by the inventory ID) to the bucket
      operationId: put-bucket-inventory-configuration
      x-api-path-slug: inventoryampidconfigurationid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
  /?inventory&amp;id=inventory-configuration-ID:
    delete:
      summary: DELETE Bucket inventory configuration
      description: This implementation of the DELETE operation deletes an inventory
        configuration(identified by the inventory configuration ID) from the bucket
      operationId: delete-bucket-inventoryconfiguration
      x-api-path-slug: inventoryampidinventoryconfigurationid-delete
      parameters:
      - in: query
        name: id
        description: The ID that identifies the inventory configuration
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
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