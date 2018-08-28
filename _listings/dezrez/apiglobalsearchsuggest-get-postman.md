{
  "info": {
    "name": "Dezrez Auto complete global search",
    "_postman_id": "a61126fd-e4b3-4e14-86f8-2b80229bbcd8",
    "description": "Auto complete global search.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auto",
      "item": [
        {
          "id": "7b492554-e94d-4f08-b109-41bd5e87e30e",
          "name": "GlobalSearch_SuggestBytextBysuggestSize",
          "request": {
            "url": "http://api.dezrez.com/api/globalsearch/suggest?suggestSize=%7B%7D&text=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Auto complete global search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2234380d-72f9-4cd0-bd53-bdbf16fdb39b"
            }
          ]
        }
      ]
    }
  ]
}