swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/sku/inventory:
    get:
      summary: Get Catalog Sku Inventory
      description: Get catalog sku inventory.
      operationId: getCatalogSkuInventory
      x-api-path-slug: catalogskuinventory-get
      parameters:
      - in: query
        name: id
        description: id
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Inventory