swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scim/v2/Users:
    get:
      summary: search or list users
      description: ""
      operationId: searchViaGet
      x-api-path-slug: scimv2users-get
      parameters:
      - in: query
        name: count
        description: page size
      - in: query
        name: filter
        description: only support userName or email filter expressions for now
      - in: query
        name: startIndex
        description: start index (1-based)
      responses:
        200:
          description: OK
      tags:
      - Search
      - List
      - Users
  /scim/v2/Users/.search:
    post:
      summary: search or list users
      description: ""
      operationId: searchViaPost
      x-api-path-slug: scimv2users-search-post
      parameters:
      - in: body
        name: body
        description: search parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - List
      - Users