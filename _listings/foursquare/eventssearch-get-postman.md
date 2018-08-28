{
  "info": {
    "name": "Foursquare Get Events Search",
    "_postman_id": "974acb5d-adfe-4abe-a746-566afa560af7",
    "description": "/events/categories",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "a2dea101-5a73-46e5-a943-46afc6654786",
          "name": "eventsevent-id",
          "request": {
            "url": "http://api.foursquare.com/v2/events/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/{EVENT_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13e7b769-1f65-4ce9-a17e-57aaf49b8518"
            }
          ]
        },
        {
          "id": "94e2d1bb-084b-4786-be4b-e89c3762fa31",
          "name": "eventscategories",
          "request": {
            "url": "http://api.foursquare.com/v2/events/search?domain=%7B%7D&eventId=%7B%7D&participantId=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2a75d35-10d6-4239-859f-5154885cf8f3"
            }
          ]
        }
      ]
    }
  ]
}