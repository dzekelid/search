---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get one customer saved search by ID
  description: Get one customer saved search by id.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/customer_saved_searches.json:
    post:
      summary: Create a new Customer Saved Search
      description: Create a new customer saved search.
      operationId: postAdminCustomerSavedSearches.json
      x-api-path-slug: admincustomer-saved-searches-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Customer
      - Saved
      - Search
  /admin/customer_saved_searches/2029905294.json:
    put:
      summary: Update an existing Customer Saved Search
      description: Update an existing customer saved search.
      operationId: putAdminCustomerSavedSearches2029905294.json
      x-api-path-slug: admincustomer-saved-searches2029905294-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Customer
      - Saved
      - Search
    delete:
      summary: Delete an existing Customer Saved Search
      description: Delete an existing customer saved search.
      operationId: deleteAdminCustomerSavedSearches2029905294.json
      x-api-path-slug: admincustomer-saved-searches2029905294-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Customer
      - Saved
      - Search
  /admin/customer_saved_searches/1189248515.json:
    get:
      summary: Get one customer saved search by ID
      description: Get one customer saved search by id.
      operationId: getAdminCustomerSavedSearches1189248515.json
      x-api-path-slug: admincustomer-saved-searches1189248515-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customer
      - Saved
      - Search
      - By
      - ID
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