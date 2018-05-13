{
  "info": {
    "name": "Giphy Gif API Search GIFs",
    "_postman_id": "033b2e78-a765-4021-b78f-6c02715df7ef",
    "description": "Search all GIPHY GIFs for a word or phrase. Punctuation will be stripped and ignored.  Use a plus or url encode for phrases. Example paul+rudd, ryan+gosling or american+psycho.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "gifs",
      "item": [
        {
          "id": "430ba4dd-4328-4268-9d3f-e3c257e82b2b",
          "name": "searchGifs",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/search?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search all GIPHY GIFs for a word or phrase"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ce23d38-f4a2-4fe9-b8b8-d19fc6209695"
            }
          ]
        }
      ]
    }
  ]
}