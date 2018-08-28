swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 1
info:
  title: Financial Crimes Insight for Insurance public REST APIs
  description: these-are-the-financial-crimes-insight-for-insurance-public-rest-apis-used-by-clients-to-access-the-fcii-capabilities
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/entitysearch:
    post:
      summary: Search for objects that match the search terms specified.
      description: 'Search for objects that match the search terms specified.  The
        searchType refers to the type of object being searched for. Valid values include:
        Folio,Account,Event,Group,PhysicalObject,Party,Transaction,Any. Note that
        paging and ordering is not supported for type Any.  The parameter globalsearch
        represents a global search string with support for the * wildcard.  The propertysearch
        fields are a list of searches for matching on specified fields of an object.'
      operationId: entitySearch
      x-api-path-slug: ibmfciplatformfactentitysearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Searchobjects
      - That
      - Match
      - Search
      - Terms
      - Specified