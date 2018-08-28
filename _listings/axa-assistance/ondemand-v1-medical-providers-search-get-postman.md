{
  "info": {
    "name": "AXA Assistance Search for medical providers",
    "_postman_id": "98caac5e-ef5e-4fb4-bf6c-f82cbf4d9f47",
    "description": "Search for medical providers",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "ed45198c-2373-40ae-b095-83dcea1fce6d",
          "name": "getOndemandV1Medical_providersSearch",
          "request": {
            "url": "http://sandbox.api.axa-assistance.com/ondemand/v1/medical_providers/search?kind=%7B%7D&lat=%7B%7D&lng=%7B%7D&speciality=%7B%7D",
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
            "description": "Search for medical providers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47697694-944e-48a5-9f22-03309783db40"
            }
          ]
        }
      ]
    }
  ]
}