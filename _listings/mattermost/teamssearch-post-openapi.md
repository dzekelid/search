---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Search teams
  description: |-
    Search teams based on search term provided in the request body.
    ##### Permissions
    Logged in user only shows open teams
    Logged in user with "manage_system" permission shows all teams
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/search:
    post:
      summary: Search users
      description: |-
        Get a list of users based on search criteria provided in the request body. Searches are typically done against username, full name, nickname and email unless otherwise configured by the server.
        ##### Permissions
        Requires an active session and `read_channel` and/or `view_team` permissions for any channels or teams specified in the request body.
      operationId: get-a-list-of-users-based-on-search-criteria-provided-in-the-request-body-searches-are-typically-don
      x-api-path-slug: userssearch-post
      parameters:
      - in: body
        name: body
        description: Search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Users
  /users/tokens/search:
    post:
      summary: Search tokens
      description: |-
        Get a list of tokens based on search criteria provided in the request body. Searches are done against the token id, user id and username.

        __Minimum server version__: 4.7

        ##### Permissions
        Must have `manage_system` permission.
      operationId: get-a-list-of-tokens-based-on-search-criteria-provided-in-the-request-body-searches-are-done-against
      x-api-path-slug: userstokenssearch-post
      parameters:
      - in: body
        name: body
        description: Search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Tokens
  /teams/search:
    post:
      summary: Search teams
      description: |-
        Search teams based on search term provided in the request body.
        ##### Permissions
        Logged in user only shows open teams
        Logged in user with "manage_system" permission shows all teams
      operationId: search-teams-based-on-search-term-provided-in-the-request-body-permissionslogged-in-user-only-shows-
      x-api-path-slug: teamssearch-post
      parameters:
      - in: body
        name: body
        description: Search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Teams
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