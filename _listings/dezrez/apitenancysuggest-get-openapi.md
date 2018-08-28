---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Search for tenancies/tennets/landlords that match the specified search
    criteria
  version: 1.0.0
  description: Search for tenancies/tennets/landlords that match the specified search
    criteria.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/agency/apikey:
    post:
      summary: Issues an API key for use with the simple role/search endpoints
      description: Issues an api key for use with the simple role/search endpoints.
      operationId: Agency_IssueApiKeyBysubjectId
      x-api-path-slug: apiagencyapikey-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subjectId
        description: The Id of the group to assign a key to
      responses:
        200:
          description: OK
      tags:
      - Issues
      - Keyuse
      - Simple
      - Role
      - Search
      - Endpoints
  /api/documentgeneration/searchmergefields:
    get:
      summary: Search Merge Fields
      description: Search merge fields.
      operationId: DocumentGeneration_SearchMergeFieldsBypartialName
      x-api-path-slug: apidocumentgenerationsearchmergefields-get
      parameters:
      - in: query
        name: partialName
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Search
      - Merge
      - Fields
  /api/globalsearch/suggest:
    get:
      summary: Auto complete global search
      description: Auto complete global search.
      operationId: GlobalSearch_SuggestBytextBysuggestSize
      x-api-path-slug: apiglobalsearchsuggest-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: suggestSize
      - in: query
        name: text
        description: Text to search on
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Complete
      - Global
      - Search
  /api/GlobalSearch:
    get:
      summary: The main endpoint for a global search across all entities in the system.
      description: The main endpoint for a global search across all entities in the
        system..
      operationId: GlobalSearch_IndexBytermByexcludeDeletedByexcludeArchivedBylastUpdated
      x-api-path-slug: apiglobalsearch-get
      parameters:
      - in: query
        name: excludeArchived
      - in: query
        name: excludeDeleted
      - in: query
        name: lastUpdated
        description: Get results from the last updated date
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: term
        description: Search term
      responses:
        200:
          description: OK
      tags:
      - The
      - Main
      - Endpointa
      - Global
      - Search
      - Across
      - ""
      - Entities
      - In
      - System
  /api/group/{id}/savesalessearch:
    post:
      summary: Saves Search Criteria to a Group
      description: Saves search criteria to a group.
      operationId: Group_SaveSalesSearchByidBysearchDataContract
      x-api-path-slug: apigroupidsavesalessearch-post
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchDataContract
        description: The groups search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Search
      - Criteria
      - To
      - Group
  /api/group/{id}/savelettingssearch:
    post:
      summary: Saves Lettings Search Criteria to a group
      description: Saves lettings search criteria to a group.
      operationId: Group_SaveLettingsSearchByidBysearchingDataContract
      x-api-path-slug: apigroupidsavelettingssearch-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchingDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Lettings
      - Search
      - Criteria
      - To
      - Group
  /api/group/{id}/deletesearch/{searchingRoleId}:
    delete:
      summary: Deletes Search Criteria from a Group
      description: Deletes search criteria from a group.
      operationId: Group_DeleteSearchByidBysearchingRoleId
      x-api-path-slug: apigroupiddeletesearchsearchingroleid-delete
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: searchingRoleId
        description: The id of the searching role to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Search
      - Criteria
      - From
      - Group
  /api/people/searchcontacts:
    post:
      summary: Search contacts based on the phone number provided
      description: Search contacts based on the phone number provided.
      operationId: People_SearchContactsBysearchCommandDataContract
      x-api-path-slug: apipeoplesearchcontacts-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchCommandDataContract
        description: Search data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Contacts
      - Based
      - "On"
      - Phone
      - Number
      - Provided
  /api/property/suggest:
    get:
      summary: Search for properties/addresses that match the specified search criteria
      description: Search for properties/addresses that match the specified search
        criteria.
      operationId: Property_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumberBydataContract.s
      x-api-path-slug: apipropertysuggest-get
      parameters:
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: query
        name: dataContract.suggestType
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchproperties
      - Addresses
      - That
      - Match
      - Specified
      - Search
      - Criteria
  /api/role/suggest:
    get:
      summary: Search for property marketing roles that match the specified search
        criteria
      description: Search for property marketing roles that match the specified search
        criteria.
      operationId: Role_SuggestBydataContract.isOnMarketBydataContract.pageNumberBydataContract.pageSizeBydataContract.
      x-api-path-slug: apirolesuggest-get
      parameters:
      - in: query
        name: dataContract.isOnMarket
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: query
        name: dataContract.roleType
      - in: query
        name: dataContract.suggestType
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchproperty
      - Marketing
      - Roles
      - That
      - Match
      - Specified
      - Search
      - Criteria
  /api/admin/searchsync/start:
    post:
      summary: Create and run as search sync request
      description: Create and run as search sync request.
      operationId: SearchSync_CreateAndStartWorkflowSyncBymigrationId
      x-api-path-slug: apiadminsearchsyncstart-post
      parameters:
      - in: query
        name: migrationId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Run
      - As
      - Search
      - Sync
      - Request
  /api/tenancy/suggest:
    get:
      summary: Search for tenancies/tennets/landlords that match the specified search
        criteria
      description: Search for tenancies/tennets/landlords that match the specified
        search criteria.
      operationId: Tenancy_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumber
      x-api-path-slug: apitenancysuggest-get
      parameters:
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchtenancies
      - Tennets
      - Landlords
      - That
      - Match
      - Specified
      - Search
      - Criteria
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