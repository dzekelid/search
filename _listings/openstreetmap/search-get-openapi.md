---
swagger: "2.0"
x-collection-name: OpenStreetMap
x-complete: 0
info:
  title: OpenStreetMap OSM - Search
  description: '[Full documentation](http://wiki.openstreetmap.org/wiki/Nominatim#Search)'
  version: 1.0.0
host: ' http:'
basePath: //nominatim.openstreetmap.org
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: OSM - Search
      description: '[Full documentation](http://wiki.openstreetmap.org/wiki/Nominatim#Search)'
      operationId: SearchGet
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: format
      - in: query
        name: q
      responses:
        200:
          description: OK
      tags:
      - Maps
      - OSM
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