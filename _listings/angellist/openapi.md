swagger: "2.0"
x-collection-name: AngelList
x-complete: 1
info:
  title: AngelList
  description: the-angellist-api-provides-developers-with-a-restful-interface-to-the-angellist-data-set--for-more-information-read-the-oauth-faq-
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Search AngelList
      description: Search AngelList.
      operationId: search
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: query
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search
  /search/slugs:
    get:
      summary: Search Slugs
      description: Search by slug
      operationId: search
      x-api-path-slug: searchslugs-get
      parameters:
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search
  /startups:
    get:
      summary: Search Startups
      description: Search Startups
      operationId: startups
      x-api-path-slug: startups-get
      parameters:
      - in: query
        name: filter
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search