---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Catalog Search
  description: Get catalog search.
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
  /catalog/search:
    get:
      summary: Get Catalog Search
      description: Get catalog search.
      operationId: getCatalogSearch
      x-api-path-slug: catalogsearch-get
      parameters:
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: page
        description: page
      - in: query
        name: pageSize
        description: pageSize
      - in: query
        name: q
        description: q
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Search
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