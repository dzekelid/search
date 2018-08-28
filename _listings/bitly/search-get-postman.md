{
  "info": {
    "name": "Bitly Link API Get Search",
    "_postman_id": "d5e68f59-6d7b-47f2-949b-cb273c740046",
    "description": "Get search.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "35fb76cc-2011-422b-a6ef-d11dfa51ce90",
          "name": "getSearch",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/search?cities=%7B%7D&domain=%7B%7D&fields=%7B%7D&full_domain=%7B%7D&lang=%7B%7D&limit=%7B%7D&offset=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afe2914c-2370-492e-baf8-ba7b7bee8eb7"
            }
          ]
        }
      ]
    }
  ]
}