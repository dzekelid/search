swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 1
info:
  title: Transport for London Unified
  description: our-unified-api-brings-together-data-across-all-modes-of-transport-into-a-single-restful-api--this-api-provides-access-to-the-most-highly-requested-realtime-and-status-infomation-across-all-the-modes-of-transport-in-a-single-and-consistent-way--access-to-the-developer-documentation-is-available-at-httpsapi-tfl-gov-uk
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /BikePoint/Search:
    get:
      summary: Bike Point  Search
      description: "Search for bike stations by their name, a bike point's name often
        contains information about the name of the street\r\n            or nearby
        landmarks, for example. note that the search result does not contain the placeproperties
        i.e. the status\r\n     ."
      operationId: BikePoint_Search
      x-api-path-slug: bikepointsearch-get
      parameters:
      - in: query
        name: query
        description: The search term e
      responses:
        200:
          description: OK
      tags:
      - Bike
      - Point
      - ""
      - Search
  /Cabwise/search:
    get:
      summary: Cabwise search
      description: Gets taxis and minicabs contact information.
      operationId: Cabwise_Get
      x-api-path-slug: cabwisesearch-get
      parameters:
      - in: query
        name: forceXml
        description: Force Xml
      - in: query
        name: lat
        description: Latitude
      - in: query
        name: legacyFormat
        description: Legacy Format
      - in: query
        name: lon
        description: Longitude
      - in: query
        name: maxResults
        description: An optional parameter to limit the number of results return
      - in: query
        name: name
        description: Trading name of operating company
      - in: query
        name: optype
        description: Operator Type e
      - in: query
        name: radius
        description: The radius of the bounding circle in metres
      - in: query
        name: twentyFourSevenOnly
        description: Twenty Four Seven Only
      - in: query
        name: wc
        description: Wheelchair accessible
      responses:
        200:
          description: OK
      tags:
      - Cabwise
      - Search
  /Line/Search/{query}:
    get:
      summary: Line  Search query
      description: Search for lines or routes matching the query string.
      operationId: Line_Search
      x-api-path-slug: linesearchquery-get
      parameters:
      - in: query
        name: modes
        description: Optionally filter by the specified modes
      - in: path
        name: query
        description: Search term e
      - in: query
        name: serviceTypes
        description: A comma seperated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Search
      - Query
  /Place/Search:
    get:
      summary: Place  Search
      description: Gets all places that matches the given query.
      operationId: Place_Search
      x-api-path-slug: placesearch-get
      parameters:
      - in: query
        name: name
        description: The name of the place, you can use the /Place/Types/{types} endpoint
          to get a list of places for a given type including their names
      - in: query
        name: types
        description: A comma-separated list of the types to return
      responses:
        200:
          description: OK
      tags:
      - Place
      - ""
      - Search
  /Search:
    get:
      summary: Search
      description: "Search the site for occurrences of the query string. the maximum
        number of results returned is equal to the maximum page size\r\n            of
        100. to return subsequent pages, use the paginated overload.."
      operationId: Search_Get
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: query
        description: The search query
      responses:
        200:
          description: OK
      tags:
      - Search
  /Search/BusSchedules:
    get:
      summary: Search  Bus Schedules
      description: Searches the bus schedules folder on s3 for a given bus number..
      operationId: Search_BusSchedules
      x-api-path-slug: searchbusschedules-get
      parameters:
      - in: query
        name: query
        description: The search query
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Bus
      - Schedules
  /Search/Meta/Categories:
    get:
      summary: Search  Meta  Categories
      description: Gets the available search categories..
      operationId: Search_MetaCategories
      x-api-path-slug: searchmetacategories-get
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Meta
      - ""
      - Categories
  /Search/Meta/SearchProviders:
    get:
      summary: Search  Meta  Search Provers
      description: Gets the available searchprovider names..
      operationId: Search_MetaSearchProviders
      x-api-path-slug: searchmetasearchproviders-get
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Meta
      - ""
      - Search
      - Provers
  /Search/Meta/Sorts:
    get:
      summary: Search  Meta  Sorts
      description: Gets the available sorting options..
      operationId: Search_MetaSorts
      x-api-path-slug: searchmetasorts-get
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Meta
      - ""
      - Sorts
  /StopPoint/Search:
    get:
      summary: Stop Point  Search
      description: Search stoppoints by their common name, or their 5-digit countdown
        bus stop code..
      operationId: StopPoint.Search.get
      x-api-path-slug: stoppointsearch-get
      parameters:
      - in: query
        name: faresOnly
        description: True to only return stations in that have Fares data available
          for single fares to another station
      - in: query
        name: includeHubs
        description: If true, returns results including HUBs
      - in: query
        name: lines
        description: An optional, parameter separated list of the lines to filter
          by
      - in: query
        name: maxResults
        description: An optional result limit, defaulting to and with a maximum of
          50
      - in: query
        name: modes
        description: An optional, parameter separated list of the modes to filter
          by
      - in: query
        name: query
        description: The query string, case-insensitive
      - in: query
        name: tflOperatedNationalRailStationsOnly
        description: If the national-rail mode is included, this flag will filter
          the national rail stations so that only those operated by TfL are returned
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Search
  /StopPoint/Search/{query}:
    get:
      summary: Stop Point  Search query
      description: Search stoppoints by their common name, or their 5-digit countdown
        bus stop code..
      operationId: StopPoint.Search.query.get
      x-api-path-slug: stoppointsearchquery-get
      parameters:
      - in: query
        name: faresOnly
        description: True to only return stations in that have Fares data available
          for single fares to another station
      - in: query
        name: includeHubs
        description: If true, returns results including HUBs
      - in: query
        name: lines
        description: An optional, parameter separated list of the lines to filter
          by
      - in: query
        name: maxResults
        description: An optional result limit, defaulting to and with a maximum of
          50
      - in: query
        name: modes
        description: An optional, parameter separated list of the modes to filter
          by
      - in: path
        name: query
        description: The query string, case-insensitive
      - in: query
        name: tflOperatedNationalRailStationsOnly
        description: If the national-rail mode is included, this flag will filter
          the national rail stations so that only those operated by TfL are returned
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Search
      - Query