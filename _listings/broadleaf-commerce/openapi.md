swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/search:
    get:
      summary: Get Catalog Search
      description: Get catalog search.
      operationId: getCatalogSearch
      x-api-path-slug: catalogsearch-get
      parameters:
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: page
        description: page
      - in: query
        name: pageSize
        description: pageSize
      - in: query
        name: q
        description: q
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Search
  /catalog/search/category/{categoryId}:
    get:
      summary: Get Catalog Search Category
      description: Get catalog search category.
      operationId: getCatalogSearchCategoryCategory
      x-api-path-slug: catalogsearchcategorycategoryid-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: page
        description: page
      - in: query
        name: pageSize
        description: pageSize
      - in: query
        name: q
        description: q
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Search
      - Category