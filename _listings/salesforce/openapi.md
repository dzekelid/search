swagger: "2.0"
x-collection-name: Salesforce
x-complete: 1
info:
  title: Salesforce Sandbox
  description: create-sandbox-copies-of-your-environments-for-development-testing-and-training-without-compromising-the-data-and-applications-in-your-production-environment-
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/search:
    get:
      summary: Get Version Search
      description: Executes the specified SOSL search. The search string must be URL-encoded.
      operationId: getVersionSearch
      x-api-path-slug: versionsearch-get
      parameters:
      - in: query
        name: q
        description: A SOSL statement
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Search