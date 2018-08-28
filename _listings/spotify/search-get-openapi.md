---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 0
info:
  title: Spotify Search
  description: '[Search for an Item](https://developer.spotify.com/web-api/search-item/)'
  version: v1
host: api.spotify.com
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
      summary: Search
      description: '[Search for an Item](https://developer.spotify.com/web-api/search-item/)'
      operationId: search-for-an-itemhttpsdeveloperspotifycomwebapisearchitem
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: offset
        description: The index of the first item to return
      - in: query
        name: q
        description: The search querys keywords (and optional field filters)
      - in: query
        name: type
        description: A comma-separated list of item types to search across
      responses:
        200:
          description: OK
      tags:
      - Music
      - Search
x-streamrank:
  polling_total_time_average: "0.1"
  polling_size_download_average: "4080.73"
  streaming_total_time_average: "0.06"
  streaming_size_download_average: "2046.76"
  change_yes: "4"
  change_no: "195"
  time_percentage: "45"
  size_percentage: "50"
  change_percentage: "2"
  last_run: "2018-05-06"
  days_run: "1"
  minute_run: "0"
---