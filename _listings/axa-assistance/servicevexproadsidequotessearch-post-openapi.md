---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Search quotes for a roadside service.
  description: Search quotes for a roadside service.
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/vexp/roadside/quotes/search:
    post:
      summary: Search quotes for a roadside service.
      description: Search quotes for a roadside service.
      operationId: postServiceVexpRoadsideQuotesSearch
      x-api-path-slug: servicevexproadsidequotessearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Search
      - quotesa
      - roadside
      - service.
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