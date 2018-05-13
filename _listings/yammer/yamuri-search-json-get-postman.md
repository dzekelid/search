{
  "info": {
    "name": "Yammer API Search Request",
    "_postman_id": "5ec4c68c-ac08-43a4-b1bf-bbdbb62d1825",
    "description": "The search resource will return a list of messages, users, topics and groups that match the user’s search query.\n\n\n\nsearch - The search query.\n\npage - Only 20 results of each type will be returned for each page, but a total count is returned with each query. page=1 (the default) will return items 1-20, page=2 will return items 21-30, etc.\n\nnum_per_page - This allows you to limit the number of results of each type per page, up to a maximum of 20, the default value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "search request",
      "item": [
        {
          "id": "5ff09faf-f134-4d3d-9bf5-2ad985b67faf",
          "name": "Search Request_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/search.json"
              ],
              "query": [
                {
                  "key": "num_per_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "yamURI",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "\tThe search resource will return a list of messages, users, topics and groups that match the user’s search query"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0758f72-66bf-4590-91ec-d808070778e4"
            }
          ]
        }
      ]
    }
  ]
}