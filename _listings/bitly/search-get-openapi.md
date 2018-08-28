---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Link API Get Search
  description: Get search.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: "3.0"
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/search:
    get:
      summary: Get Search
      description: Search links receiving clicks across bitly by content, language,
        location, and more.
      operationId: Get_realtime_search_
      x-api-path-slug: v3search-get
      parameters:
      - in: query
        name: cities
        description: (optional) show links active in this city (ordered like country-state-city,
          e
      - in: query
        name: domain
        description: (optional) restrict results to this web domain
      - in: query
        name: format
        description: Response format
      - in: query
        name: lang
        description: (optional) favor results in this language (two letter ISO code)
      - in: query
        name: limit
        description: (optional) the maximum number of links to return
      - in: query
        name: offset
        description: (optional) which result to start with (defaults to 0)
      - in: query
        name: query
        description: string to query for
      responses:
        200:
          description: OK
      tags:
      - Search
  /search:
    get:
      summary: Get Search
      description: Get search.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: cities
        description: show links active in this city (ordered like country-state-city,
          e
      - in: query
        name: domain
        description: restrict results to this web domain (like bitly
      - in: query
        name: fields
        description: which fields to return in the response (comma-separated)
      - in: query
        name: full_domain
        description: restrict results to this full web domain (like blog
      - in: query
        name: lang
        description: favor results in this language (two letter ISO code)
      - in: query
        name: limit
      - in: query
        name: offset
        description: which result to start with (defaults to 0)
      - in: query
        name: query
        description: string to query for
      responses:
        200:
          description: OK
      tags:
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