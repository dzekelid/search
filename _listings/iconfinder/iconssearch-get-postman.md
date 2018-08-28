{
  "info": {
    "name": "Icon Finder Search for icons",
    "_postman_id": "50b49838-965c-4da6-9569-353f806c84c3",
    "description": "Search through icons by various criteria. The returned list of icons is ordered descendingly by popularit",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Authors",
      "item": [
        {
          "id": "863daa6e-4e0a-4efc-939d-796a224a66f0",
          "name": "getAuthorsAuthor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "authors/:authorID"
              ],
              "query": [
                {
                  "key": "authors",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "authorID",
                  "value": "authorID",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific author identified by a unique ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34af33d5-e7ce-402a-bb9a-170dd21bea34"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "24a085d9-753d-4a0f-9933-e101e257a160",
          "name": "getCategories",
          "request": {
            "url": "http://api.iconfinder.com/v2/categories?after=%7B%7D&count=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all categories sorted ascendingly by their identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9da15908-02d9-4e4d-a48c-5162146507a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Icons",
      "item": [
        {
          "id": "8455e8d7-5ee2-4a9a-82a1-6ca8564623eb",
          "name": "getIconsSearch",
          "request": {
            "url": "http://api.iconfinder.com/v2/icons/search?category=%7B%7D&count=%7B%7D&license=%7B%7D&maximum_size=%7B%7D&minimum_size=%7B%7D&offset=%7B%7D&premium=%7B%7D&query=%7B%7D&style=%7B%7D&vector=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search through icons by various criteria. The returned list of icons is ordered descendingly by popularit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94eacda2-db5f-4e79-aed4-2d7946e8a1d0"
            }
          ]
        }
      ]
    }
  ]
}