{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - All Data Combined ECHO Facility Enhanced Search Service",
    "_postman_id": "13ebf6fc-7b01-4b74-825d-ac338c55c63c",
    "description": "Returns either an array of Facilities or an array of Clusters that meet the specified search criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "3e15f3b2-a483-4e3b-a9c7-021789e98152",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/echo_rest_services.get_download?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return a comma sepated vaule (CSV) file of the facilities found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "cd3b8ee4-2a78-49b7-b82a-69b199dc1fd3"
        }
      ]
    },
    {
      "id": "249ac612-1fd2-4d29-9842-b245618d165e",
      "name": "validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/echo_rest_services.get_facilities?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Validates query search parameters and returns query identifier.  Use the responseset parameter to set the page size"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d3d2436d-65a2-4477-86d3-d48f66ecc958"
        }
      ]
    },
    {
      "id": "bfd10933-54b4-4f9f-bbcb-8d55082ee72e",
      "name": "returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/echo_rest_services.get_facility_info?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns either an array of Facilities or an array of Clusters that meet the specified search criteria."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "898bb646-6976-4ead-bb57-0a25d62b89dc"
        }
      ]
    }
  ]
}