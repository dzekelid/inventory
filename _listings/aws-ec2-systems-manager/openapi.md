---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetInventory:
    get:
      summary: Get Inventory
      description: Query inventory information.
      operationId: getInventory
      x-api-path-slug: actiongetinventory-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: ResultAttributes
        description: The list of inventory item types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
  /?Action=GetInventorySchema:
    get:
      summary: Get Inventory Schema
      description: |-
        Return a list of inventory type names for the account, or return a list of attribute
           names for a specific Inventory item type.
      operationId: getInventorySchema
      x-api-path-slug: actiongetinventoryschema-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TypeName
        description: The type of inventory item to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
      - Schema
  /?Action=ListInventoryEntries:
    get:
      summary: List Inventory Entries
      description: A list of inventory items returned by the request.
      operationId: listInventoryEntries
      x-api-path-slug: actionlistinventoryentries-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: InstanceId
        description: The instance ID for which you want inventory information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TypeName
        description: The type of inventory item for which you want information
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Inventory
      - Entries
  /?Action=PutInventory:
    get:
      summary: Put Inventory
      description: Bulk update custom inventory items on one more instance.
      operationId: putInventory
      x-api-path-slug: actionputinventory-get
      parameters:
      - in: query
        name: InstanceId
        description: One or more instance IDs where you want to add or update inventory
          items
        type: string
      - in: query
        name: Items
        description: The inventory items that you want to add or update on instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
---