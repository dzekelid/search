---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Get Lat / Log
  description: Given a latitude and a longitude, searches for up to 20 places that
    can be used as a place_id when updatting a status
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /saved_searches/list:
    get:
      summary: List Saved Searches
      description: Returns the authenticated user's saved search queries
      operationId: returns-the-authenticated-users-saved-search-queries
      x-api-path-slug: saved-searcheslist-get
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /saved_searches/show/{id}:
    get:
      summary: Get Saved Search
      description: Retrieve the information for the saved search represented by the
        given id
      operationId: retrieve-the-information-for-the-saved-search-represented-by-the-given-id
      x-api-path-slug: saved-searchesshowid-get
      parameters:
      - in: path
        name: id
        description: The id of the saved search
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /saved_searches/create:
    post:
      summary: Create Saved Search
      description: Create a new saved search for the authenticated user
      operationId: create-a-new-saved-search-for-the-authenticated-user
      x-api-path-slug: saved-searchescreate-post
      parameters:
      - in: query
        name: query
        description: The query of the search the user would like to save
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /saved_searches/destroy/{id}:
    post:
      summary: Destroy Saved Search
      description: Destroy a saved search for the authenticating user
      operationId: destroy-a-saved-search-for-the-authenticating-user
      x-api-path-slug: saved-searchesdestroyid-post
      parameters:
      - in: path
        name: id
        description: The id of the saved search
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /geo/reverse_geoncode:
    get:
      summary: Get Lat / Log
      description: Given a latitude and a longitude, searches for up to 20 places
        that can be used as a place_id when updatting a status
      operationId: given-a-latitude-and-a-longitude-searches-for-up-to-20-places-that-can-be-used-as-a-place-id-when-up
      x-api-path-slug: georeverse-geoncode-get
      parameters:
      - in: query
        name: accuracy
        description: A hint on region in which to search
      - in: query
        name: callback
        description: If supplied, the responses will use the JSON format with a callback
          of the given name
      - in: query
        name: granularity
        description: This is the minimal granularity of place types to return
      - in: query
        name: lat
        description: The latitude to search around
      - in: query
        name: long
        description: The longtitude to search around
      - in: query
        name: max_results
        description: A hint as to the number of results to return
      responses:
        200:
          description: OK
      tags:
      - Places
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