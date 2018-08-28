swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 1
info:
  title: IDX API 1.4.0 Test Runner
  description: idx-broker-api-calls-in-version-1-4-0required-environment-variable-url-environment-variable-for-request-headers-environment-variable-partner-key-client-account-with-at-least-one-featured-listingtests-are-in-this-order-as-variables-such-as-listing-id-and-approved-mls-are-passed-to-subsequent-api-calls-
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mls/searchfieldvalues/{approvedMLS}:
    get:
      summary: Get Mls Search Field Values Approved MLS
      description: Field values in a given MLS that are currently allowed to be searched
        according to MLS guidelines.
      operationId: MlsSearchfieldvaluesByApprovedMLSGet
      x-api-path-slug: mlssearchfieldvaluesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: query
        name: mlsPtID
      - in: query
        name: name
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Search
      - Field
      - Values
      - Approved
      - MLS
  /clients/searchquery:
    get:
      summary: Get Search Query
      description: Performs search and returns the results.
      operationId: ClientsSearchqueryGet
      x-api-path-slug: clientssearchquery-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Search
      - Query
  /leads/search/{leadId}:
    get:
      summary: Get Leads Search
      description: Get saved search information for a lead.
      operationId: LeadsSearchByLeadIdGet
      x-api-path-slug: leadssearchleadid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search
    put:
      summary: Put Leads Search
      description: New search information for a lead.
      operationId: LeadsSearchByLeadIdPut
      x-api-path-slug: leadssearchleadid-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: formData
        name: searchName
      - in: formData
        name: search[hp]
      - in: formData
        name: search[idxID]
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search
  /leads/search/{leadId}/{searchId}:
    post:
      summary: Post Leads Search
      description: Update search information for a lead.
      operationId: LeadsSearchByLeadIdAndSearchIdPost
      x-api-path-slug: leadssearchleadidsearchid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: path
        name: searchId
      - in: formData
        name: searchName
      - in: formData
        name: search[hp]
      - in: formData
        name: search[idxID]
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search
    delete:
      summary: Delete Leads Search
      description: Delete search information for a lead.
      operationId: LeadsSearchByLeadIdAndSearchIdDelete
      x-api-path-slug: leadssearchleadidsearchid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: path
        name: searchId
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search