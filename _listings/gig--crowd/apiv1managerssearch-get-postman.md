{
  "info": {
    "name": "GIGANDCROWD Get Managers Search",
    "_postman_id": "8b4e9715-7aa5-4103-897b-8ae1d6d22b3a",
    "description": "Get managers search.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Managers",
      "item": [
        {
          "id": "9dba856b-7c30-4938-ab79-50abff048dac",
          "name": "getApiV1ManagersSettings",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/managers/settings",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get managers settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cb4aaac-c3f0-4b45-a1df-e2caae075585"
            }
          ]
        },
        {
          "id": "eaa27e38-4423-493b-b68b-fdc5d2cc17dc",
          "name": "getApiV1ManagersSearch",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/managers/search?request.query=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get managers search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fd2170f-b2e4-4d71-b109-498a542eadc2"
            }
          ]
        }
      ]
    }
  ]
}