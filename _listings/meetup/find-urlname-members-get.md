---
swagger: "2.0"
info:
  title: Meetup Group Profile search
  description: |-
    Find group member profiles by name.
    Member's who very recently joined or left the group may not be immediately searchable
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /find/:urlname/members:
    get:
      summary: Group Profile search
      description: Find group member profiles by name
      operationId: profiles
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: order
        description: Orders results according to definitions listed below
        type: string
      - in: query
        name: page
        description: Number of requested members to return
        type: string
      - in: query
        name: query
        description: The name to search for
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - groups
      - search
definitions: []
x-collection-name: Meetup
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