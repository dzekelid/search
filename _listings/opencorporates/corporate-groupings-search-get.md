---
swagger: "2.0"
info:
  title: OpenCorporates Corporate Groupings Search
  description: nThis returns a collection of corporate_groupings whose name matches
    the given search term (submitted as :q in the query parameters)
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /corporate_groupings/search:
    get:
      summary: Corporate Groupings Search
      description: nThis returns a collection of corporate_groupings whose name matches
        the given search term (submitted as :q in the query parameters)
      operationId: corporate-groupings-search
      responses:
        200:
          description: OK
      tags:
      - businesses
      - corporate
      - groupings
      - search
definitions: []
x-collection-name: OpenCorporates
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