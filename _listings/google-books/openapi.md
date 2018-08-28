swagger: "2.0"
x-collection-name: Google Books
x-complete: 1
info:
  title: Books
  description: searches-for-books-and-manages-your-google-books-library-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /volumes:
    get:
      summary: Book Search
      description: Performs a book search.
      operationId: books.volumes.list
      x-api-path-slug: volumes-get
      parameters:
      - in: query
        name: download
        description: Restrict to volumes by download availability
      - in: query
        name: filter
        description: Filter search results
      - in: query
        name: langRestrict
        description: Restrict results to books with this language code
      - in: query
        name: libraryRestrict
        description: Restrict search to this users library
      - in: query
        name: maxAllowedMaturityRating
        description: The maximum allowed maturity rating of returned recommendations
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: orderBy
        description: Sort search results
      - in: query
        name: partner
        description: Restrict and brand results for partner ID
      - in: query
        name: printType
        description: Restrict to books or magazines
      - in: query
        name: projection
        description: Restrict information returned to a set of selected fields
      - in: query
        name: q
        description: Full-text search query string
      - in: query
        name: showPreorders
        description: Set to true to show books available for preorder
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first result to return (starts at 0)
      responses:
        200:
          description: OK
      tags:
      - Search