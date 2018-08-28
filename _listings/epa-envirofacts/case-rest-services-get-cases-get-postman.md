{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Enforcement Case Search Enforcement Case Search",
    "_postman_id": "688c695b-e8e1-40e6-b550-5148045d6eac",
    "description": "The get_cases service end point searches for civil enforcement and criminal cases based on the provided selection criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "de529d6a-a9b7-4a70-8547-92fad95bf902",
      "name": "the-get-case-report-service-endpoint-returns-a-complex-object-of-civil-enforcement-case-details-base",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/case_rest_services.get_case_report?No Name=%7B%7D&output=%7B%7D&p_id=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The get_case_report service endpoint returns a complex object of civil enforcement case details based on the provided case id."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "4aa00e6d-d3e0-4384-9a89-ac2e025f5644"
        }
      ]
    },
    {
      "id": "5dc3c2fd-ca12-4138-a2b1-fe88dc8b64c5",
      "name": "the-get-cases-service-end-point-searches-for-civil-enforcement-and-criminal-cases-based-on-the-provi",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/case_rest_services.get_cases?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The get_cases service end point searches for civil enforcement and criminal cases based on the provided selection criteria."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "4a54d63f-5f58-428f-9147-38e4a67d4669"
        }
      ]
    }
  ]
}