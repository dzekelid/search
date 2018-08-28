{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - All Data Combined ECHO Facility Search Service",
    "_postman_id": "fc2b195c-9b41-45de-860f-a4d9692e586b",
    "description": "Validates query search parameters and returns query identifier.  Use the responseset parameter to set the page size",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "c995c0a4-5bc4-43f1-9279-9f09621f5ec8",
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
          "id": "b40f01d9-1422-426a-9806-5a7e6fada7b5"
        }
      ]
    },
    {
      "id": "339d0028-b970-43a1-b696-ade30b8254b4",
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
          "id": "0cfd1874-a49a-4ed4-9953-4d06232ff64e"
        }
      ]
    }
  ]
}