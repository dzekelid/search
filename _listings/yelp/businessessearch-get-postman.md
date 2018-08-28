{
  "info": {
    "name": "Yelp Get Businesses Search",
    "_postman_id": "1e59295f-0d22-45d2-91cd-5988dd8145b9",
    "description": "Get businesses search.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Businesses",
      "item": [
        {
          "id": "f8be48b6-b2c7-486f-8720-fae8a616ff40",
          "name": "getBusinessesSearch",
          "request": {
            "url": "http://api.yelp.com/v3/businesses/search?No Name=%7B%7D&term=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get businesses search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6deb7255-457c-4e42-b667-79a993b705ef"
            }
          ]
        }
      ]
    }
  ]
}