---
swagger: "2.0"
x-collection-name: BetterDoctor
x-complete: 0
info:
  title: BetterDoctor Doctor search
  description: Doctor search
  version: 1.0.0
host: api.betterdoctor.com
basePath: /2016-03-01
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /doctors:
    get:
      summary: Doctor search
      description: Doctor search
      operationId: doctor-search
      x-api-path-slug: doctors-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: first_name
        description: The doctors first name; partial (type-ahead) characters/names
          are accepted
      - in: query
        name: gender
        description: The doctors gender (male or female)
      - in: query
        name: insurance_uid
        description: UID of an insurance plan (e
      - in: query
        name: last_name
        description: The doctors last name; partial (type-ahead) characters/names
          are accepted
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: location
        description: Search area - Either Circular (lat,lon,range (miles)) or Bounding
          box (top-right, bottom-left) (lat,lon,lat,lon)
      - in: query
        name: name
        description: The doctors name; searches in both first and last names
      - in: query
        name: practice_uid
        description: BetterDoctor Practice UID
      - in: query
        name: query
        description: Search all fields by a keyword query (e
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: sort
        description: 'Sort order for the search results (full-name-asc: Alphabetical
          sort by full provider name ascending'
      - in: query
        name: specialty_uid
        description: UID of a specialty (e
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: user_location
        description: Users current location
      responses:
        200:
          description: OK
      tags:
      - Doctor
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