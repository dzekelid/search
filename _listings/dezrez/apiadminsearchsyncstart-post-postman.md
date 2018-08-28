{
  "info": {
    "name": "Dezrez Create and run as search sync request",
    "_postman_id": "0399091f-2e16-472b-9ea9-88020bc07a95",
    "description": "Create and run as search sync request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Run",
      "item": [
        {
          "id": "ddbc1695-3a20-4abf-b7aa-f192cf6ea097",
          "name": "SearchSync_CreateAndStartWorkflowSyncBymigrationId",
          "request": {
            "url": "http://api.dezrez.com/api/admin/searchsync/start?migrationId=%7B%7D",
            "method": "POST",
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
            "description": "Create and run as search sync request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1acaaaeb-d6fc-41ee-8367-535b38324f3d"
            }
          ]
        }
      ]
    }
  ]
}