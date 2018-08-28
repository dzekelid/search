---
swagger: "2.0"
x-collection-name: Public Transport Victoria Timetable
x-complete: 0
info:
  title: PTV Timetable API - Version 3 Get V3 Search Search Term
  description: View stops, routes and myki ticket outlets that match the search term.
  termsOfService: http://ptv.vic.gov.au/ptv-timetable-api/
  contact:
    name: Public Transport Victoria
    url: http://ptv.vic.gov.au/digital
  version: v3
host: timetableapi.ptv.vic.gov.au
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/search/{search_term}:
    get:
      summary: Get V3 Search Search Term
      description: View stops, routes and myki ticket outlets that match the search
        term.
      operationId: Search_Search
      x-api-path-slug: v3searchsearch-term-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: include_addresses
        description: Placeholder for future development; currently unavailable
      - in: query
        name: include_outlets
        description: Indicates if outlets will be returned in response (default =
          true)
      - in: query
        name: latitude
        description: Filter by geographic coordinate of latitude
      - in: query
        name: longitude
        description: Filter by geographic coordinate of longitude
      - in: query
        name: max_distance
        description: Filter by maximum distance (in metres) from location specified
          via latitude and longitude parameters
      - in: query
        name: route_types
        description: 'Filter by route_type; values returned via RouteTypes API (note:
          stops and routes are ordered by route_types specified)'
      - in: path
        name: search_term
        description: 'Search text (note: if search text is numeric and/or less than
          3 characters, the API will only return routes)'
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Search
      - Search
      - Term
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