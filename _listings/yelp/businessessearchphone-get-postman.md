{
  "info": {
    "name": "Yelp Get Businesses Search Phone",
    "_postman_id": "80b25995-fe8e-48e0-83a8-24806c91ab71",
    "description": "Get businesses search phone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Businesses",
      "item": [
        {
          "id": "bb35b699-2fe5-4c67-b6a1-e642b448d0e9",
          "name": "getBusinessesSearch",
          "request": {
            "url": "http://api.yelp.com/v3/businesses/search?No Name=%7B%7D&term=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get businesses search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a64e6cc9-0808-42b4-b17f-cc3becf7471f"
            }
          ]
        },
        {
          "id": "d0bf1824-ccda-4ac4-8fec-9b25c2ca345c",
          "name": "getBusinesses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.yelp.com",
              "path": [
                "v3",
                "businesses/:id"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get businesses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35f84a09-4ede-4802-9503-5192c011d9c1"
            }
          ]
        },
        {
          "id": "2afa6af6-8bdc-47dd-96fb-38a723d29022",
          "name": "getBusinessesReviews",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.yelp.com",
              "path": [
                "v3",
                "businesses/:id/reviews"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get businesses reviews."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d927aca-c73d-4427-8817-62c595be331b"
            }
          ]
        },
        {
          "id": "630d957d-f016-478c-841c-35c4f6ebea5c",
          "name": "getBusinessesSearchPhone",
          "request": {
            "url": "http://api.yelp.com/v3/businesses/search/phone?No Name=%7B%7D&phone=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get businesses search phone."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0ebefff-c88c-46a5-b83c-d4081b7cf77f"
            }
          ]
        }
      ]
    }
  ]
}