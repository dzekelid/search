swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /legacy/issues/search/{owner}/{repository}/{state}/{keyword}:
    get:
      summary: Get Legacy Issues Search Owner Repository State Keyword
      description: Find issues by state and keyword.
      operationId: find-issues-by-state-and-keyword
      x-api-path-slug: legacyissuessearchownerrepositorystatekeyword-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: keyword
        description: The search term
      - in: path
        name: owner
      - in: path
        name: repository
      - in: path
        name: state
        description: Indicates the state of the issues to return
      responses:
        200:
          description: OK
      tags:
      - Legacy
      - Issues
      - Search
      - Owner
      - Repository
      - State
      - Keyword
  /legacy/repos/search/{keyword}:
    get:
      summary: Get Legacy Repos Search Keyword
      description: Find repositories by keyword. Note, this legacy method does not
        follow the v3 pagination pattern. This method returns up to 100 results per
        page and pages can be fetched using the start_page parameter.
      operationId: find-repositories-by-keyword-note-this-legacy-method-does-not-follow-the-v3-pagination-pattern-this-
      x-api-path-slug: legacyrepossearchkeyword-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: keyword
        description: The search term
      - in: query
        name: language
        description: Filter results by language
      - in: query
        name: order
        description: The sort field
      - in: query
        name: sort
        description: The sort field
      - in: query
        name: start_page
        description: The page number to fetch
      responses:
        200:
          description: OK
      tags:
      - Legacy
      - Repos
      - Search
      - Keyword
  /legacy/user/search/{keyword}:
    get:
      summary: Get Legacy User Search Keyword
      description: Find users by keyword.
      operationId: find-users-by-keyword
      x-api-path-slug: legacyusersearchkeyword-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: keyword
        description: The search term
      - in: query
        name: order
        description: The sort field
      - in: query
        name: sort
        description: The sort field
      - in: query
        name: start_page
        description: The page number to fetch
      responses:
        200:
          description: OK
      tags:
      - Legacy
      - User
      - Search
      - Keyword
  /search/code:
    get:
      summary: Get Search Code
      description: Search code.
      operationId: search-code
      x-api-path-slug: searchcode-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: order
        description: The sort field
      - in: query
        name: q
        description: The search terms
      - in: query
        name: sort
        description: Can only be indexed, which indicates how recently a file has
          been indexedby the GitHub search infrastructure
      responses:
        200:
          description: OK
      tags:
      - Search
      - Code
  /search/issues:
    get:
      summary: Get Search Issues
      description: Find issues by state and keyword. (This method returns up to 100
        results per page.)
      operationId: find-issues-by-state-and-keyword-this-method-returns-up-to-100-results-per-page
      x-api-path-slug: searchissues-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: order
        description: The sort field
      - in: query
        name: q
        description: 'The q search term can also contain any combination of the supported
          issue search qualifiers:'
      - in: query
        name: sort
        description: The sort field
      responses:
        200:
          description: OK
      tags:
      - Search
      - Issues
  /search/repositories:
    get:
      summary: Get Search Repositories
      description: Search repositories.
      operationId: search-repositories
      x-api-path-slug: searchrepositories-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: order
        description: The sort field
      - in: query
        name: q
        description: The search terms
      - in: query
        name: sort
        description: If not provided, results are sorted by best match
      responses:
        200:
          description: OK
      tags:
      - Search
      - Repositories
  /search/users:
    get:
      summary: Get Search Users
      description: Search users.
      operationId: search-users
      x-api-path-slug: searchusers-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: order
        description: The sort field
      - in: query
        name: q
        description: The search terms
      - in: query
        name: sort
        description: If not provided, results are sorted by best match
      responses:
        200:
          description: OK
      tags:
      - Search
      - Users