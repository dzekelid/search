---
swagger: "2.0"
x-collection-name: BC Geographical Names
x-complete: 0
info:
  title: BC Geographical Names Search by name, limit to unofficial names only
  description: Search for information about unofficial geographical names by the text
    of the name itself.  Various options and filter parameters are available to refine
    the search.
  contact:
    name: BC Geographical Names Office
    email: geographical.names@gov.bc.ca
  version: 3.x.x
host: apps.gov.bc.ca
basePath: /pub/bcgnws
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /names/notOfficial/search:
    get:
      summary: Search by name, limit to unofficial names only
      description: Search for information about unofficial geographical names by the
        text of the name itself.  Various options and filter parameters are available
        to refine the search.
      operationId: search-for-information-about-unofficial-geographical-names-by-the-text-of-the-name-itself---various-
      x-api-path-slug: namesnotofficialsearch-get
      parameters:
      - in: query
        name: embed
        description: A flag to indicate whether to embed the corresponding feature
          into each matching name
      - in: query
        name: exactSpelling
        description: If the name parameter is specified, exactSpelling specifies whether
          to include only names that exactly match the search text (exactSpelling=1),
          or whether to also include names with similar spellings (exactSpelling=0)
      - in: query
        name: featureCategory
        description: A filter to limit the search to names associated with features
          of a certain category  The value of this parameter should be a featureCategoryCode
          value returned by the /featureCategories resource, or an asterisk (*) to
          request that all feature categories be included
      - in: query
        name: featureClass
        description: A filter to limit the search to names associated with features
          of a certain class  The value of this parameter should be a featureClassCode
          value returned by the /featureClasses resource, or an asterisk (*) to request
          that all feature classes be included
      - in: query
        name: featureType
        description: A filter to limit the search to names associated with features
          of a certain type  The value of this parameter should be a featureTypeCode
          value returned by the /featureTypes resource, or an asterisk (*) to request
          that all feature types be included
      - in: query
        name: itemsPerPage
        description: The number of search results to return (1-200)
      - in: query
        name: name
        description: A filter to search based on the the text of the name itself
      - in: query
        name: outputFormat
        description: The format of the output
      - in: query
        name: outputSRS
        description: The EPSG code of the spatial reference system (SRS) to use for
          output geometries
      - in: query
        name: outputStyle
        description: A flag indicating whether to include with each matching name
          a succinct list of attributes (summary), or a comprehensive list of attributes
          (detail)
      - in: query
        name: sortBy
        description: The distance to move the accessPoint away from the curb and towards
          the inside of the parcel (in metres)
      - in: query
        name: startIndex
        description: The index of the first record to be returned (>= 1)
      responses:
        200:
          description: OK
      tags:
      - Names
      - NotOfficial
      - Search
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