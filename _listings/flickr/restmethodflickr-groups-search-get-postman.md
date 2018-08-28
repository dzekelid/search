{
  "info": {
    "name": "Flickr Groups Search",
    "_postman_id": "195c6799-c007-44fa-af33-c97909670b31",
    "description": "Search for groups. 18+ groups will only be returned for authenticated calls where the authenticated user is over 18.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "7f551834-38da-46ef-ba6e-42276e5af95c",
          "name": "getRestMethodFlickr.groups.browse",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.browse?api_key=%7B%7D&cat_id=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Browse the group category tree, finding groups and sub-categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aea740d8-797d-4390-8aba-ec46bffaf7ee"
            }
          ]
        },
        {
          "id": "a35301f5-4019-4e8e-85fd-dddf7e5d8075",
          "name": "getRestMethodFlickr.groups.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.getInfo?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&lang=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8037084-e902-4499-afca-a7580d9d0ca7"
            }
          ]
        },
        {
          "id": "ddca6508-2e23-4abd-8efb-19081aedb1df",
          "name": "getRestMethodFlickr.groups.search",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.search?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&text=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for groups. 18+ groups will only be returned for authenticated calls where the authenticated user is over 18."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3ca5a61-a390-4b62-9e35-261400ed8fc0"
            }
          ]
        }
      ]
    }
  ]
}