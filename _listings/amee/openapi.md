swagger: "2.0"
x-collection-name: AMEE
x-complete: 1
info:
  title: AMEE WRI Aqueduct API
  version: 1.0.0
host: api.roaring.io
basePath: /company/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /company-simple-search:
    get:
      summary: Get Company Simple Search
      description: Get company simple search.
      operationId: getCompanySimpleSearch
      x-api-path-slug: companysimplesearch-get
      parameters:
      - in: query
        name: companyName
        description: Company name
      - in: query
        name: countryCode
        description: Country code for the company
      - in: query
        name: town
        description: Town
      responses:
        200:
          description: OK
      tags:
      - Company
      - Simple
      - Search