{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation and Recovery Act  Resource Conservation and Recovery Act (RCRA) Facility Search Service",
    "_postman_id": "e216a390-256d-4e73-9399-03e78b08670c",
    "description": "Validates query search parameters and returns query identifier.  Use the responseset parameter to set the page size",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "63a37edc-2bc9-4978-825f-03b15edd0773",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
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
          "id": "62ef0515-badb-495b-b2fd-bba89eccd55c"
        }
      ]
    },
    {
      "id": "3958ee52-d956-4995-a1b4-48c29b9f3fba",
      "name": "validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_facilities?No Name=%7B%7D&output=%7B%7D",
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
          "id": "52a3892b-f30d-42a9-8ac1-9d5a02385b22"
        }
      ]
    }
  ]
}