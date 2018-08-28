swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Searching for Content
      description: The search endpoint provides a powerful way of finding items that
        are accessible by a single user or an entire enterprise. Leverage the parameters
        listed below to generate targeted advanced searches.
      operationId: search
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: ancestor_folder_ids
        description: Limit searches to specific parent folders
      - in: query
        name: content_types
        description: Limit searches to specific Box designated content types
      - in: query
        name: created_at_range
        description: The date for when the item was created
      - in: query
        name: file_extensions
        description: Limit searches to specific file extensions like pdf,png,doc
      - in: query
        name: limit
        description: Number of search results to return
      - in: query
        name: mdfilters
        description: Filters for a specific metadata template for files with metadata
          object associations
      - in: query
        name: offset
        description: The search result at which to start the response
      - in: query
        name: owner_user_ids
        description: Search by item owners
      - in: query
        name: query
        description: The string to search for; can be matched against item names,
          descriptions, text content of a file, and other fields of the different
          item types
      - in: query
        name: scope
        description: The scope for which you want to limit your search to
      - in: query
        name: size_range
        description: Filter by a file size range
      - in: query
        name: trash_content
        description: Allows you to search within the trash
      - in: query
        name: type
        description: The type you want to return in your search
      - in: query
        name: updated_at_range
        description: The date for when the item was last updated
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Search