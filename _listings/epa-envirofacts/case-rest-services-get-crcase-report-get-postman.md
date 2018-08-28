{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Enforcement Case Search Enforcement Criminal Case Summary Report Search",
    "_postman_id": "8fe96a31-5c8a-4047-a1ed-26d5a10d755c",
    "description": "The get_crcase_report service end point returns a complex object of criminal case detials based on the provided criminal case id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "aca7b28f-c41a-42e7-955b-b2e9ec2e88c9",
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
          "id": "0f80698b-5a95-46f7-b2fe-c1b00b7b0bbf"
        }
      ]
    },
    {
      "id": "5b574845-79cc-455a-9359-d141dbdc0a18",
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
          "id": "192ecfe7-a9b0-4a83-b43c-9ba812776826"
        }
      ]
    },
    {
      "id": "4820a017-7370-4b4f-87a7-67e7e187f956",
      "name": "the-get-crcase-report-service-end-point-returns-a-complex-object-of-criminal-case-detials-based-on-t",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/case_rest_services.get_crcase_report?No Name=%7B%7D&output=%7B%7D&p_id=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The get_crcase_report service end point returns a complex object of criminal case detials based on the provided criminal case id."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "913c3a11-6078-4f63-b020-b0afa8c88d3b"
        }
      ]
    }
  ]
}