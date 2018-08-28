swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/follows/search:
    get:
      summary: Get My Follows Search
      description: Follow status for a search
      operationId: getMyFollowsSearch
      x-api-path-slug: myfollowssearch-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Search
    post:
      summary: Post My Follows Search
      description: Post my follows search.
      operationId: postMyFollowsSearch
      x-api-path-slug: myfollowssearch-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Search