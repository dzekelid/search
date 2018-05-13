---
swagger: "2.0"
info:
  title: Google Doubleclick API Search
  version: 1.0.0
  description: Gets the requested product.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products/search:
    get:
      summary: Search
      description: Gets the requested product
      operationId: adexchangebuyer.products.search
      parameters:
      - in: query
        name: pqlQuery
        description: The pql query used to query for products
      responses:
        200:
          description: OK
      tags:
      - advertising
      - search
definitions: []
x-collection-name: Google Doubleclick
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