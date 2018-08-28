swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  search/{mediaType}:
    get:
      summary: Get Search Mediatype
      description: Search news
      operationId: getSearchMediatype
      x-api-path-slug: searchmediatype-get
      parameters:
      - in: query
        name: apiKey
        description: API Key
      - in: query
        name: arrivalDate
        description: The date when the content item was released, in the format  YYYY-MM-DD,
          YYYY-MM, YYYY or YYYY-MM-DDTHH:mmZ where the value must be in Coordinated
          Universal Time  (UTC)
      - in: query
        name: contentSet
        description: The AP Images content set to be searched
      - in: query
        name: count
        description: The number of search results per page
      - in: query
        name: creationDate
        description: The date when the content item was created, in the format  YYYY-MM-DD,
          YYYY-MM, YYYY or YYYY-MM-DDTHH:mmZ where the value must be in Coordinated
          Universal Time  (UTC)
      - in: query
        name: event
        description: One or more words from the title of a specific event
      - in: query
        name: imageId
        description: One or more image ID numbers assigned to content items
      - in: query
        name: locations
        description: A geographic location in the AP Geography vocabulary
      - in: path
        name: mediaType
        description: The content media type (photo, graphic, video)
      - in: query
        name: metadataLevel
        description: The level of metadata to be included in search results
      - in: query
        name: page
        description: The page number within the set of search results
      - in: query
        name: person
        description: The name of a person who is featured in the content item
      - in: query
        name: photographer
        description: The photographers first and/or last name
      - in: query
        name: q
        description: The search query
      - in: query
        name: showParametrics
        description: By default, query facets that allow you to refine the original  search
          are returned for each content item at the entry level only
      - in: query
        name: sortby
        description: Specifies how to sort the search results
      - in: query
        name: source
        description: One or more content creators
      - in: query
        name: subject
        description: Subject category in the AP Subject vocabulary
      - in: query
        name: transref
        description: Transmission reference number
      responses:
        200:
          description: OK
      tags:
      - Search
      - Mediatype