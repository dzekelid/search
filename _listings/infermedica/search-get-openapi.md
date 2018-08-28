---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 0
info:
  title: Infermedica Get Search
  description: Returns list of observations matching the given phrase.
  version: v2
host: api.infermedica.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Get Search
      description: Returns list of observations matching the given phrase.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: max_results
        description: maximum number of results
      - in: query
        name: phrase
        description: phrase to match
      - in: query
        name: sex
        description: sex filter
      - in: query
        name: type
        description: type of results
      responses:
        200:
          description: OK
      tags:
      - Healthcare
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