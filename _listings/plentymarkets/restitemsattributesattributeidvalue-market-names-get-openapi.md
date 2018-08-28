---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Search attribute value market names
  description: Search attribute value market names.
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