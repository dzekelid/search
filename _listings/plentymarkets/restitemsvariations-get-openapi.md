---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Search variations
  description: Search variations by different filters
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/delete_log:
    get:
      summary: Search the delete log
      description: Searches the delete log.
      operationId: getRestDeleteLog
      x-api-path-slug: restdelete-log-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
        description: The type of deleted record
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to deleteLogs updated during
          the specified period
      - in: query
        name: userId
        description: The ID of the user who deleted the record
      responses:
        200:
          description: OK
      tags:
      - Search
      - Delete
      - Log
  /rest/items:
    get:
      summary: Search item
      description: Search item.
      operationId: getRestItems
      x-api-path-slug: restitems-get
      parameters:
      - in: query
        name: flagOne
        description: Filter restricts the list of results to items with the specified
          flagOne
      - in: query
        name: flagTwo
        description: Filter restricts the list of results to items with the specified
          flagTwo
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to items with the specified
          manufacturerId
      - in: query
        name: name
        description: Filter restricts the list of results to items with the specified
          item name
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: tagId
        description: Filter restricts the list of results to items with the specified
          tagId
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to items updated during
          the specified period
      - in: query
        name: variationRelatedUpdatedBetween
        description: Filter restricts the list of results to items with variations
          for which related information was updated during the specified period
      - in: query
        name: variationUpdatedBetween
        description: Filter restricts the list of results to items with variations
          that were updated during the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - Search
      - Item
  /rest/items/attributes/{attributeId}/value_market_names:
    get:
      summary: Search attribute value market names
      description: Search attribute value market names.
      operationId: getRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lang
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
      responses:
        200:
          description: OK
      tags:
      - Search
      - Attribute
      - Value
      - Market
      - Names
  /rest/items/variations:
    get:
      summary: Search variations
      description: Search variations by different filters
      operationId: getRestItemsVariations
      x-api-path-slug: restitemsvariations-get
      parameters:
      - in: query
        name: barcode
        description: Filter restricts the list of results to variations with the specified
          barcode
      - in: query
        name: categoryId
        description: Filter restricts the list of results to variations with the specified
          category id
      - in: query
        name: createdBetween
        description: Filter restricts the list of results to variations created during
          the specified period
      - in: query
        name: flagOne
        description: Filter restricts the list of results to variations of items with
          the flag one
      - in: query
        name: flagTwo
        description: Filter restricts the list of results to variations of items with
          the flag two
      - in: query
        name: id
        description: Filter restricts the list of results to variations with the specified
          variation ID
      - in: query
        name: isActive
        description: Filter restricts the list of results to variations that are active
      - in: query
        name: isBundle
        description: Filter restricts the list of results to variations to which variations
          were added to create a bundle
      - in: query
        name: isMain
        description: Filter restricts the list of results to variations that are main
          variations
      - in: query
        name: itemId
        description: Filter restricts the list of results to variations with the specified
          item ID
      - in: query
        name: itemName
        description: Filter restricts the list of results to variations with the specified
          item name
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: itemTagId
        description: Filter restricts the list of results to variations with the specified
          tag ID
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to variations with the specified
          manufacturer ID
      - in: query
        name: numberExact
        description: Filter restricts the list of results to the variation with the
          variation number specified
      - in: query
        name: numberFuzzy
        description: Filter restricts the list of results to variations with numbers
          that contain the variation number specified (SQL LIKE operator)
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: plentyId
        description: Filter restricts the list of results to variations to which variations
          were visible in specific Clients
      - in: query
        name: relatedUpdatedBetween
        description: Filter restricts the list of results to those variations for
          which related information was updated during the specified period
      - in: query
        name: sku
        description: Filter restricts the list of results to variations with the specified
          SKU
      - in: query
        name: storeSpecial
        description: Filter restricts the list of results to variations of items with
          the specified store special
      - in: query
        name: supplierNumber
        description: Filter restricts the list of results to variations with the specified
          supplier number
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to variations updated during
          the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - Search
      - Variations
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