swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products/search:
    get:
      summary: Search
      description: Gets the requested product.
      operationId: adexchangebuyer.products.search
      x-api-path-slug: productssearch-get
      parameters:
      - in: query
        name: pqlQuery
        description: The pql query used to query for products
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Search