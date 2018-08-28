---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Groups Search
  description: Search for groups. 18+ groups will only be returned for authenticated
    calls where the authenticated user is over 18.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.groups.search:
    get:
      summary: Groups Search
      description: Search for groups. 18+ groups will only be returned for authenticated
        calls where the authenticated user is over 18.
      operationId: getRestMethodFlickr.groups.search
      x-api-path-slug: restmethodflickr-groups-search-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of groups to return per page
      - in: query
        name: text
        description: The text to search for
      responses:
        200:
          description: OK
      tags:
      - Groups
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