---
swagger: "2.0"
x-collection-name: EU BON UTIS
x-complete: 0
info:
  title: EU BON UTIS Search
  description: Search
  termsOfService: https://www.biodiversitycatalogue.org/services/79
  version: "1.0"
host: cybertaxonomy.eu
basePath: /eu-bon/utis/1.0
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
      description: Search
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: addSynonymy
        description: Indicates whether the synonymy of the accepted taxon should be
          included into the response
      - in: query
        name: providers
        description: A list of provider id strings concatenated by comma characters
      - in: query
        name: query
        description: The scientific name to search for
      - in: query
        name: searchMode
        description: Specifies the searchMode
      - in: query
        name: timeout
        description: The maximum of milliseconds to wait for responses from any of
          the providers
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