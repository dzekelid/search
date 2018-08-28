{
  "info": {
    "name": "AXA Assistance Retrieve all medical provider kinds available for search (Ex: pharmacy, hospital ...)",
    "_postman_id": "539170ea-14d7-4288-81e0-4aef92bb4b7a",
    "description": "Retrieve all medical provider kinds available for search (Ex: pharmacy, hospital ...)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "b0e93091-ee0f-47c3-886c-132991368a9b",
          "name": "getOndemandV1Medical_providersKinds",
          "request": {
            "url": "http://sandbox.api.axa-assistance.com/ondemand/v1/medical_providers/kinds",
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
            "description": "Retrieve all medical provider kinds available for search (Ex: pharmacy, hospital "
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef3d0938-95c8-43bb-8713-712a0753558f"
            }
          ]
        }
      ]
    }
  ]
}