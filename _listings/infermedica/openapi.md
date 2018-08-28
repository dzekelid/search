swagger: "2.0"
x-collection-name: Infermedica
x-complete: 1
info:
  title: Infermedica
  description: empower-your-healthcare-services-with-intelligent-diagnostic-insights-of-infermedica-api-
  version: v2
host: api.infermedica.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Get Search
      description: Returns list of observations matching the given phrase.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: max_results
        description: maximum number of results
      - in: query
        name: phrase
        description: phrase to match
      - in: query
        name: sex
        description: sex filter
      - in: query
        name: type
        description: type of results
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Search