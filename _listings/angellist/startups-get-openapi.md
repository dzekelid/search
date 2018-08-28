---
swagger: "2.0"
x-collection-name: AngelList
x-complete: 0
info:
  title: AngelList Search Startups
  description: Search Startups
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Search AngelList
      description: Search AngelList.
      operationId: search
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: query
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search
  /search/slugs:
    get:
      summary: Search Slugs
      description: Search by slug
      operationId: search
      x-api-path-slug: searchslugs-get
      parameters:
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search
  /startups:
    get:
      summary: Search Startups
      description: Search Startups
      operationId: startups
      x-api-path-slug: startups-get
      parameters:
      - in: query
        name: filter
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
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