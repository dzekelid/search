{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Enforcement Case Search Enforcement Case Summary Report Search",
    "_postman_id": "0146e9e7-6679-45f3-8e1f-ec16bca6f23e",
    "description": "The get_case_report service endpoint returns a complex object of civil enforcement case details based on the provided case id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "3b353d62-6fe7-4b49-aeb4-5246350575cd",
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
          "id": "1f90b679-58ff-4e59-ab61-11c306bfdb07"
        }
      ]
    }
  ]
}