---
swagger: "2.0"
x-collection-name: Browshot
x-complete: 0
info:
  title: Browshot Search for screenshots
  description: Search for screenshots of a specific URL.
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /screenshot/search:
    get:
      summary: Search for screenshots
      description: Search for screenshots of a specific URL.
      operationId: SearchScreenshot
      x-api-path-slug: screenshotsearch-get
      parameters:
      - in: query
        name: limit
        description: maximum number of screenshots information to return
      - in: query
        name: status
        description: get list of screenshot in a given status (error, finished, in_process)
      - in: query
        name: url
        description: look for a string matching the URL requested
      responses:
        200:
          description: OK
      tags:
      - Screenshot
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