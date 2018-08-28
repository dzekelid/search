---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral search or list users
  description: ""
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scim/v2/Users:
    get:
      summary: search or list users
      description: ""
      operationId: searchViaGet
      x-api-path-slug: scimv2users-get
      parameters:
      - in: query
        name: count
        description: page size
      - in: query
        name: filter
        description: only support userName or email filter expressions for now
      - in: query
        name: startIndex
        description: start index (1-based)
      responses:
        200:
          description: OK
      tags:
      - Search
      - List
      - Users
  /scim/v2/Users/.search:
    post:
      summary: search or list users
      description: ""
      operationId: searchViaPost
      x-api-path-slug: scimv2users-search-post
      parameters:
      - in: body
        name: body
        description: search parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - List
      - Users
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