swagger: "2.0"
x-collection-name: NPR
x-complete: 1
info:
  title: NPR One API Reference
  description: npr-one-is-a-smart-application-that-brings-the-best-of-npr-and-member-station-programming-newscasts-podcasts-and-stories-together-to-create-a-new-experience-for-listening--it-provides-an-editorcurated-and-localized-mobile-listening-experience-based-on-the-content-the-listener-chooses-likes-shares-and-enjoys--the-api-provides-all-of-the-content-and-customization-in-a-simple-structured-way-that-is-easy-for-applicationdevelopers-to-implement-
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