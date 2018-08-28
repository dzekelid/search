---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - All Data Combined
    ECHO Facility Search Service
  description: Validates query search parameters and returns query identifier.  Use
    the responseset parameter to set the page size
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 1.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /echo_rest_services.get_facility_info:
    get:
      summary: Combined ECHO Facility Enhanced Search Service
      description: Returns either an array of Facilities or an array of Clusters that
        meet the specified search criteria.
      operationId: returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri
      x-api-path-slug: echo-rest-services-get-facility-info-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Combined
      - ECHO
      - Facility
      - Enhanced
      - Search
      - Service
  /echo_rest_services.get_facilities:
    get:
      summary: Combined ECHO Facility Search Service
      description: Validates query search parameters and returns query identifier.  Use
        the responseset parameter to set the page size
      operationId: validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se
      x-api-path-slug: echo-rest-services-get-facilities-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Combined
      - ECHO
      - Facility
      - Search
      - Service
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