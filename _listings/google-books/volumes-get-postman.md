{
  "info": {
    "name": "Google Books API Book Search",
    "_postman_id": "7677a172-4592-472f-9aee-b895a21a49c8",
    "description": "Performs a book search.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "search",
      "item": [
        {
          "id": "e52c2e8a-8e1f-46cd-9e0a-9ab8823dfe33",
          "name": "books.volumes.list",
          "request": {
            "url": "http://www.googleapis.com/books/v1/volumes?download=%7B%7D&filter=%7B%7D&langRestrict=%7B%7D&libraryRestrict=%7B%7D&maxAllowedMaturityRating=%7B%7D&maxResults=%7B%7D&orderBy=%7B%7D&partner=%7B%7D&printType=%7B%7D&projection=%7B%7D&q=%7B%7D&showPreorders=%7B%7D&source=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Performs a book search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e73b3fc3-b9b7-4be7-9d06-89ceb468911a"
            }
          ]
        }
      ]
    }
  ]
}