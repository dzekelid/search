---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR Get a list of recent audio and aggregation items associated with search
    terms
  description: In the schema shown below, SearchItemDocument is not an actual type
    of returned object; the object returned by a search will be either an AggregationAudioItemListDocument
    or an AudioItemDocument.
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listening/v2/search/recommendations:
    get:
      summary: Get a list of recent audio and aggregation items associated with search
        terms
      description: In the schema shown below, SearchItemDocument is not an actual
        type of returned object; the object returned by a search will be either an
        AggregationAudioItemListDocument or an AudioItemDocument.
      operationId: getSearchRecommendations
      x-api-path-slug: listeningv2searchrecommendations-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: searchTerms
        description: Search terms to search on; can include URL-encoded punctuation
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - Search
      - Recommendations
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---