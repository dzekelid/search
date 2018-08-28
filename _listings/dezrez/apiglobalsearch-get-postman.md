{
  "info": {
    "name": "Dezrez The main endpoint for a global search across all entities in the system.",
    "_postman_id": "57175777-fa72-4be2-9d5a-2e64c111a357",
    "description": "The main endpoint for a global search across all entities in the system..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auto",
      "item": [
        {
          "id": "5d9310e7-dd68-4ae3-b4c7-01d0e8073ab6",
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
              "id": "2bb89ea6-af46-48fc-8361-cc75642af208"
            }
          ]
        }
      ]
    },
    {
      "name": "The",
      "item": [
        {
          "id": "ce981810-7569-4352-9404-d9f61aa33045",
          "name": "GlobalSearch_IndexBytermByexcludeDeletedByexcludeArchivedBylastUpdated",
          "request": {
            "url": "http://api.dezrez.com/api/GlobalSearch?excludeArchived=%7B%7D&excludeDeleted=%7B%7D&lastUpdated=%7B%7D&term=%7B%7D",
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
            "description": "The main endpoint for a global search across all entities in the system.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "823a9804-6e7c-445d-806d-23a68b37c917"
            }
          ]
        }
      ]
    }
  ]
}