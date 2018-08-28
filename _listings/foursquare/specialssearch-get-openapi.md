---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Specials Search
  description: /specials/list
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/search:
    get:
      summary: Get Events Search
      description: /events/categories
      operationId: eventscategories
      x-api-path-slug: eventssearch-get
      parameters:
      - in: query
        name: domain
        description: Identifier for a known third-party event provider
      - in: query
        name: eventId
        description: Identifier used by third-party specifed in domain, which we will
          attempt to match against our events listings
      - in: query
        name: participantId
        description: Identifier used by third-party specifed in domain, which we will
          attempt to match against our events listings
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
  /pages/search:
    get:
      summary: Get Pages Search
      description: /pages/{PAGE_ID}
      operationId: pagespage-id
      x-api-path-slug: pagessearch-get
      parameters:
      - in: query
        name: fbid
        description: A comma-delimited list of Facebook IDs to look for
      - in: query
        name: name
        description: A search term to be applied against page names
      - in: query
        name: twitter
        description: A comma-delimited list of Twitter handles to look for
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Pages
      - Search
  /specials/search:
    get:
      summary: Get Specials Search
      description: /specials/list
      operationId: specialslist
      x-api-path-slug: specialssearch-get
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Accuracy of the users altitude, in meters
      - in: query
        name: limit
        description: Number of results to return, up to 50
      - in: query
        name: ll
        description: Latitude and longitude to search near
      - in: query
        name: llAcc
        description: Accuracy of latitude and longitude, in meters
      - in: query
        name: radius
        description: Limit results to venues within this many meters of the specified
          location
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
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