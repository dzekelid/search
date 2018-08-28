swagger: "2.0"
x-collection-name: OpenStreetMap
x-complete: 1
info:
  title: Open Street Map (OSM)
  description: todo-add-description
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