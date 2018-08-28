{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Safe Drinking Water Act Safe Drinking Water Act (SDWA) Systems Search Service",
    "_postman_id": "b0f893ab-6d21-4975-b120-6b73009b5f99",
    "description": "Returns an array of public water systems that meet the specified search criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "8a6fef51-fbb2-4732-b02e-01b4383556ca",
      "name": "based-on-the-qid-obtained-from-a-get-systems-query-return-a-comma-sepated-vaule-csv-file-of-the-wate",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/sdw_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_systems query, return a comma sepated vaule (CSV) file of the water systems found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "30350357-d157-4cf8-8330-c37b9c000c25"
        }
      ]
    },
    {
      "id": "00b6f519-5b60-442f-a26b-1e93458ad1dd",
      "name": "get-qid-is-passed-with-a-query-id-corresponding-to-a-previously-run-get-systems-query--it-then-retur",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/sdw_rest_services.get_qid?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "GET_QID is passed with a query ID corresponding to a previously run get_systems query. It then returns a Systems object containing all matching water systems. The main purpose of GET_QID is for large querysets that contain multiple pages (responsesets) of output. GET_QID allows for pagination and for the selection and sorting of columns."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "8f9e0101-388e-45d4-8844-c72e90d7e1e2"
        }
      ]
    },
    {
      "id": "39b6038f-cabc-4f09-94a1-6c31f22fea22",
      "name": "returns-an-array-of-public-water-systems-that-meet-the-specified-search-criteria-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/sdw_rest_services.get_systems?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns an array of public water systems that meet the specified search criteria."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d8f1c7ec-5421-43a3-9243-0db7f0dac525"
        }
      ]
    }
  ]
}