swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products/search.json:
    get:
      summary: Get Products Search
      description: ""
      operationId: getProductsSearch.json
      x-api-path-slug: productssearch-json-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: query
        description: Query for the Product
      responses:
        200:
          description: OK
      tags:
      - Products
      - Search
      - Json