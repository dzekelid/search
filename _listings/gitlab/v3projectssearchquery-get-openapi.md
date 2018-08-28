---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Search Query
  version: 1.0.0
  description: Search for projects the current user has access to
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/search/{query}:
    get:
      summary: Get Projects Search Query
      description: Search for projects the current user has access to
      operationId: getV3ProjectsSearchQuery
      x-api-path-slug: v3projectssearchquery-get
      parameters:
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: path
        name: query
        description: The project name to be searched
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Search
      - Query
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