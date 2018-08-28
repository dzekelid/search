{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation and Recovery Act  Resource Conservation and Recovery Act (RCRA) Facility Enhanced Search Service",
    "_postman_id": "4df0ba35-c5cf-4203-8d1f-6f7efe434532",
    "description": "Returns either an array of Facilities or an array of Clusters that meet the specified search criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "b350e707-ee1f-407c-ac4e-21af940d0582",
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
          "id": "5b7fc7d7-4b88-4987-92d4-d33d54365dd9"
        }
      ]
    },
    {
      "id": "e2b3e8d5-fbc0-4835-8cb1-6d13738ee1d2",
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
          "id": "47cfd0a1-c193-4029-9272-2b38085de046"
        }
      ]
    },
    {
      "id": "57ed1152-f54e-4ff3-91c2-6d2a45980fdb",
      "name": "returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_facility_info?No Name=%7B%7D&output=%7B%7D",
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
          "id": "5be48d2c-8317-4fd8-aec3-54ac25efd41b"
        }
      ]
    }
  ]
}