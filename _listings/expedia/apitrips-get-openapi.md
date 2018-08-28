---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Get Trips
  description: Mobile API Trips
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/trips:
    get:
      summary: Get Trips
      description: Mobile API Trips
      operationId: trips-search
      x-api-path-slug: apitrips-get
      parameters:
      - in: query
        name: filterBookingStatus
        description: An optional parameter to filter by booking status
      - in: query
        name: filterLineOfBusiness
        description: An optional parameters to filter by line of business
      - in: query
        name: filterTimePeriod
        description: An optional parameter to filter by time period
      - in: query
        name: getCachedDetails
        description: Optionally get full details for the first N trips
      - in: query
        name: sort
        description: An optional parameter to sort by date
      responses:
        200:
          description: OK
      tags:
      - Travel
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