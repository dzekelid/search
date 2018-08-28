{
  "info": {
    "name": "AXA Assistance Retrieve all medical provider specialities available for search (Ex: cardiology, dentist ...)",
    "_postman_id": "44e57359-da9b-4849-b66c-8e39a24bf7ef",
    "description": "Retrieve all medical provider specialities available for search (Ex: cardiology, dentist ...)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "43600c65-126c-487a-9f60-0f54f66f4c2c",
          "name": "getOndemandV1Medical_providersSpecialities",
          "request": {
            "url": "http://sandbox.api.axa-assistance.com/ondemand/v1/medical_providers/specialities",
            "method": "GET",
            "header": [
              {
                "key": "accept-language",
                "value": "{}",
                "description": "Language/Country",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all medical provider specialities available for search (Ex: cardiology, dentist "
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "946846c2-193e-4e20-9e4d-cc3f20e98eca"
            }
          ]
        }
      ]
    }
  ]
}