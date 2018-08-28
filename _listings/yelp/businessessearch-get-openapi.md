---
swagger: "2.0"
x-collection-name: Yelp
x-complete: 0
info:
  title: Yelp Get Businesses Search
  description: Get businesses search.
  version: 1.0.0
host: api.yelp.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /businesses/search:
    get:
      summary: Get Businesses Search
      description: Get businesses search.
      operationId: getBusinessesSearch
      x-api-path-slug: businessessearch-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: term
      responses:
        200:
          description: OK
      tags:
      - Businesses
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