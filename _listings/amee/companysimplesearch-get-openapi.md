---
swagger: "2.0"
x-collection-name: AMEE
x-complete: 0
info:
  title: AMEE Company API Get Company Simple Search
  description: Get company simple search.
  version: "1.0"
host: api.roaring.io
basePath: /company/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /company-simple-search:
    get:
      summary: Get Company Simple Search
      description: Get company simple search.
      operationId: getCompanySimpleSearch
      x-api-path-slug: companysimplesearch-get
      parameters:
      - in: query
        name: companyName
        description: Company name
      - in: query
        name: countryCode
        description: Country code for the company
      - in: query
        name: town
        description: Town
      responses:
        200:
          description: OK
      tags:
      - Company
      - Simple
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