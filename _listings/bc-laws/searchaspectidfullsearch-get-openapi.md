---
swagger: "2.0"
x-collection-name: BC Laws
x-complete: 0
info:
  title: BC Laws A listing of metadata available for the specified aspect and search
    term from the BCLaws legislative repository
  description: A listing of metadata available for the specified aspect and search
    term from the BCLaws legislative repository
  termsOfService: http://www.data.gov.bc.ca/local/dbc/docs/license/API_Terms_of_Use.pdf
  version: 1.0.0
host: www.bclaws.ca
basePath: /civix
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /document/id/{aspectId}/{civixIndexId}/{civixDocumentId}/search/{searchString}:
    get:
      summary: Retrieves a specific document from the BCLaws legislative repository
        with search text highlighted (HTML format)
      description: 'The /document API allows you to retrieve actual documents from
        the BCLaws legislative repository. To retrieve a document from the repository
        you need the aspect identifier and two other specific pieces of information
        about the document: the index identifier and the document identifier. These
        unique identifiers can be retrieved from the /content API.'
      operationId: getDocumentAspectCivixindexCivixdocumentSearchSearchstring
      x-api-path-slug: documentidaspectidcivixindexidcivixdocumentidsearchsearchstring-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      - in: path
        name: civixIndexId
        description: Index identification code
      - in: path
        name: searchString
        description: The text to search for within the document
      responses:
        200:
          description: OK
      tags:
      - Document
      - Id
      - AspectId
      - CivixIndexId
      - CivixDocumentId
      - Search
      - SearchString
  /document/id/{aspectId}/{civixIndexId}/{civixDocumentId}/xml/search/{searchString}:
    get:
      summary: Retrieves a specific document from the BCLaws legislative repository
        with search text highlighted (XML format)
      description: 'The /document API allows you to retrieve actual documents from
        the BCLaws legislative repository. To retrieve a document from the repository
        you need the aspect identifier and two other specific pieces of information
        about the document: the index identifier and the document identifier. These
        unique identifiers can be retrieved from the /content API.'
      operationId: getDocumentAspectCivixindexCivixdocumentXmlSearchSearchstring
      x-api-path-slug: documentidaspectidcivixindexidcivixdocumentidxmlsearchsearchstring-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      - in: path
        name: civixIndexId
        description: Index identification code
      - in: path
        name: searchString
        description: The text to search for within the document
      responses:
        200:
          description: OK
      tags:
      - Document
      - Id
      - AspectId
      - CivixIndexId
      - CivixDocumentId
      - Xml
      - Search
      - SearchString
  /search/{aspectId}/fullsearch:
    get:
      summary: A listing of metadata available for the specified aspect and search
        term from the BCLaws legislative repository
      description: A listing of metadata available for the specified aspect and search
        term from the BCLaws legislative repository
      operationId: getSearchAspectFullsearch
      x-api-path-slug: searchaspectidfullsearch-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: query
        name: e
        description: last hit (end index)
      - in: query
        name: lFrag
        description: length of fragment snippets (< 200)
      - in: query
        name: nFrag
        description: number of fragment snippets to return (< 10)
      - in: query
        name: q
        description: query term
      - in: query
        name: s
        description: first hit (start index)
      responses:
        200:
          description: OK
      tags:
      - Search
      - AspectId
      - Fullsearch
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