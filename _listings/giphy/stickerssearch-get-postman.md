{
  "info": {
    "name": "Giphy Gif API Search Stickers",
    "_postman_id": "7c6043af-0570-4eb5-9638-799a485b0854",
    "description": "Replicates the functionality and requirements of the classic GIPHY search, but returns animated stickers rather than GIFs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "stickers",
      "item": [
        {
          "id": "c6b26c6b-b74e-4ad9-8ef8-097e9f6e27bb",
          "name": "searchStickers",
          "request": {
            "url": "http://api.giphy.com/v1/stickers/search?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Replicates the functionality and requirements of the classic GIPHY search, but returns animated stickers rather than GIFs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4de6804-a207-4fc0-b2ea-bbae7a9b703e"
            }
          ]
        }
      ]
    }
  ]
}