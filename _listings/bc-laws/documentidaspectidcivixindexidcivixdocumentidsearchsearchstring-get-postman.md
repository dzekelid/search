{
  "info": {
    "name": "BC Laws Retrieves a specific document from the BCLaws legislative repository with search text highlighted (HTML format)",
    "_postman_id": "db342ccf-3155-46cc-ab53-3f747af3e5b1",
    "description": "The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Content",
      "item": [
        {
          "id": "bc2bf335-a67c-4f9f-9595-bc73fe0ead1f",
          "name": "getContentAspectCivixdocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "content/:aspectId/:civixDocumentId"
              ],
              "variable": [
                {
                  "id": "aspectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixDocumentId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the metadata available for the specified index or directory from the BCLaws legislative respository"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2451dcdc-0cb6-4527-bb15-45680002a4b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "3071d0c9-7e44-4e93-94cd-186f7b2bd368",
          "name": "getDocumentAspectCivixindexCivixdocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "document/id/:aspectId/:civixIndexId/:civixDocumentId"
              ],
              "variable": [
                {
                  "id": "aspectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixDocumentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixIndexId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25de75b6-7485-4836-8460-3ea47d43072d"
            }
          ]
        },
        {
          "id": "ae3947a4-f630-4707-a88c-3eabb42053c7",
          "name": "getDocumentAspectCivixindexCivixdocumentSearchSearchstring",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "document/id/:aspectId/:civixIndexId/:civixDocumentId/search/:searchString"
              ],
              "variable": [
                {
                  "id": "aspectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixDocumentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixIndexId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "searchString",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad4fa5d5-bed4-47b1-8c68-8facf4bb9370"
            }
          ]
        }
      ]
    }
  ]
}