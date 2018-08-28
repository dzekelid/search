swagger: "2.0"
x-collection-name: Clearbit
x-complete: 1
info:
  title: Clearbit
  description: welcome-to-clearbits-api-you-can-use-this-api-to-access-all-our-api-endpoints-such-as-the-person-api-to-look-up-email-addresses-or-the-company-api-to-look-up-company-information-related-to-a-domain-name-
  version: 1.0.0
host: discovery.clearbit.com
basePath: /v1/companies
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Find Contacts - Job Title
      description: 'TODO: Add Description'
      operationId: SearchGet3
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: domain
      - in: query
        name: email
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Search