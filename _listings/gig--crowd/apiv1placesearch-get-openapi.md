---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Place Search
  version: 1.0.0
  description: Get place search.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/art/search/{page}:
    post:
      summary: Post Art Search Page
      description: Post art search page.
      operationId: postApiV1ArtSearchPage
      x-api-path-slug: apiv1artsearchpage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Art
      - Search
      - Page
  /api/v1/gigme/artist/search/{page}:
    post:
      summary: Post Gigme Artist Search Page
      description: Post gigme artist search page.
      operationId: postApiV1GigmeArtistSearchPage
      x-api-path-slug: apiv1gigmeartistsearchpage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Artist
      - Search
      - Page
  /api/v1/managers/search:
    get:
      summary: Get Managers Search
      description: Get managers search.
      operationId: getApiV1ManagersSearch
      x-api-path-slug: apiv1managerssearch-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: request.query
      responses:
        200:
          description: OK
      tags:
      - Managers
      - Search
  /api/v1/message/chats/{pageNumber}/{search}:
    get:
      summary: Get Message Chats Pagenumber Search
      description: Get message chats pagenumber search.
      operationId: getApiV1MessageChatsPagenumberSearch
      x-api-path-slug: apiv1messagechatspagenumbersearch-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: pageNumber
      - in: path
        name: search
      - in: query
        name: unread
      responses:
        200:
          description: OK
      tags:
      - Message
      - Chats
      - Pagenumber
      - Search
  /api/v1/place/search:
    get:
      summary: Get Place Search
      description: Get place search.
      operationId: getApiV1PlaceSearch
      x-api-path-slug: apiv1placesearch-get
      parameters:
      - in: query
        name: request.cities
      - in: query
        name: request.query
      responses:
        200:
          description: OK
      tags:
      - Place
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