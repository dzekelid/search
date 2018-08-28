---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Associate User To Trip
  description: Mobile API User Associate To Trip
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
  /api/trips/{tripId}:
    get:
      summary: Trips by tripId
      description: Mobile API Trips
      operationId: trips-search-id
      x-api-path-slug: apitripstripid-get
      parameters:
      - in: query
        name: currencyCode
        description: Currency parameter
      - in: query
        name: decimalPlaceCount
        description: Decimal place count for the expected amount
      - in: query
        name: decorator
        description: Nullifies complex elements of a Trip with exception of Price
          related elements and their parents
      - in: query
        name: email
        description: To pull a guest itinerary specify the email address associated
          with the trip
      - in: query
        name: expectedAmount
        description: Expected Amount during car cancellation
      - in: path
        name: tripId
        description: The trip ID
      - in: query
        name: useCache
        description: An optional flag to make a cached read trip call
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Search
      - Trips
  /api/trips/{tripId}/updateTripNameDescription:
    post:
      summary: Update Trip Name and Description
      description: Mobile API Trips update trip name and description operation
      operationId: trips-update-trip
      x-api-path-slug: apitripstripidupdatetripnamedescription-post
      parameters:
      - in: path
        name: tripId
        description: Trip ID
      - in: formData
        name: tripname
        description: The name of the trip
      - in: formData
        name: tripnote
        description: The comments of the trip
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Search
      - Trips
  /api/user/associateUserToTrip:
    post:
      summary: Associate User To Trip
      description: Mobile API User Associate To Trip
      operationId: user-associate-to-trip
      x-api-path-slug: apiuserassociateusertotrip-post
      parameters:
      - in: formData
        name: foo
        description: stubbed
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Search
      - Trips
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