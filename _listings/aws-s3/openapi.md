swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
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
    get:
      summary: GET Bucket inventory configuration
      description: This implementation of the GET operation returns an inventory configuration
        (identified bythe inventory configuration ID) from the bucket
      operationId: get-bucket-inventory-configuration
      x-api-path-slug: inventoryampidinventoryconfigurationid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration