{
  "info": {
    "name": "BC Laws Retrieves a specific document from the BCLaws legislative repository with search text highlighted (XML format)",
    "_postman_id": "ef80e0fe-6cb0-40d1-9533-eebed338a44e",
    "description": "The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Content",
      "item": [
        {
          "id": "d960b9c0-21f5-44d9-b68e-28a6de47126c",
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
              "id": "e9e30d1c-70dc-4f53-98b6-63c9baadcaef"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "7014c559-421d-44dc-8bbd-655e3af7a176",
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
              "id": "29e200e6-fffe-4838-aeda-fb0495b169be"
            }
          ]
        },
        {
          "id": "fc1d377d-db11-49a1-a41c-0269e569685b",
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
              "id": "a9833919-4422-491b-8fec-03d0415a2d72"
            }
          ]
        },
        {
          "id": "cbafac15-14ce-4cae-aa66-70d597b5407b",
          "name": "getDocumentAspectCivixindexCivixdocumentXml",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "document/id/:aspectId/:civixIndexId/:civixDocumentId/xml"
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
              "id": "1a246d9b-5cd2-40a4-8fee-07d024f0a666"
            }
          ]
        },
        {
          "id": "f342437c-816b-4c60-a0b2-cebecc1feea4",
          "name": "getDocumentAspectCivixindexCivixdocumentXmlSearchSearchstring",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "document/id/:aspectId/:civixIndexId/:civixDocumentId/xml/search/:searchString"
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
              "id": "5e5e406e-f80a-4b33-8917-dbfe0d09489a"
            }
          ]
        }
      ]
    }
  ]
}