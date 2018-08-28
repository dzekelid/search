swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /maps/search:
    get:
      summary: Search maps
      description: Search maps
      operationId: maps.search.get
      x-api-path-slug: mapssearch-get
      parameters:
      - in: query
        name: d
        description: Distance
      - in: query
        name: lat
        description: 'Latitude for search radius (default distance: 2000 meter)'
      - in: query
        name: lon
        description: 'Longitude for search radius (default distance: 2000 meter)'
      - in: query
        name: q
        description: Query
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Search
      - Maps
  /spots/search:
    get:
      summary: Search spots
      description: Search spots
      operationId: spots.search.get
      x-api-path-slug: spotssearch-get
      parameters:
      - in: query
        name: d
        description: Distance
      - in: query
        name: lat
        description: Latitude for search radius (2 km)
      - in: query
        name: lon
        description: Longitude for search radius (2 km)
      - in: query
        name: q
        description: Query
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Search
      - Spots
  /users/search:
    get:
      summary: Search users
      description: Search users
      operationId: users.search.get
      x-api-path-slug: userssearch-get
      parameters:
      - in: query
        name: q
        description: Query
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Search
      - Users