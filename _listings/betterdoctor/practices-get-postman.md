{
  "info": {
    "name": "BetterDoctor Practice Search",
    "_postman_id": "a75cacf3-502f-4635-99f1-d44c8e9ff367",
    "description": "Results are provider service locations, commonly referred as practices or doctor's offices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "practices",
      "item": [
        {
          "id": "27f2c5c5-0d10-479a-89d1-a74a93cc5fae",
          "name": "results-are-provider-service-locations-commonly-referred-as-practices-or-doctors-offices",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/practices?fields=%7B%7D&limit=%7B%7D&location=%7B%7D&name=%7B%7D&skip=%7B%7D&sort=%7B%7D&user_key=%7B%7D&user_location=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Results are provider service locations, commonly referred as practices or doctor's offices"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a24cc6c3-bc7a-4f4a-b426-29e121c43cde"
            }
          ]
        }
      ]
    }
  ]
}