{
  "info": {
    "name": "Bitly Domains API Get Search",
    "_postman_id": "71cefd6f-472f-4e42-a600-3c6ab92a8639",
    "description": "Search links receiving clicks across bitly by content, language, location, and more.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shorten",
      "item": [
        {
          "id": "45a7e865-3246-4db0-a842-22f825c69f1f",
          "name": "Get_shorten_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/shorten?domain=%7B%7D&format=%7B%7D&longUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a long URL, returns a bitly short URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "779c137c-6ad5-491f-9c0d-81e5d567d466"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "7b0133ff-d673-4c20-89d3-65cf5c5111ce",
          "name": "Get_expand_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a bitly URL or hash (or multiple), returns the target (long) URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9440e178-e2b6-4f30-859d-5ebc2fed4f5a"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "c8eb50ee-4799-4aa5-9616-9145a156bec9",
          "name": "Get_lookup_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/lookup?format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to query for a bitly link based on a long URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e31bbcf1-803c-4511-9d3f-9372a6f50fc2"
            }
          ]
        },
        {
          "id": "d133f2b5-f890-42d2-8e20-8ea62c782309",
          "name": "Get_link_clicks_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/clicks?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0ef3a37-da10-4a25-a5f9-674e52dfac7c"
            }
          ]
        },
        {
          "id": "1ab78318-b74e-402d-8039-c8fd7bc617bd",
          "name": "Get_link_countries_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/countries?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the countries referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "651b0c33-89b1-4db1-b967-4297758f4a90"
            }
          ]
        },
        {
          "id": "79c97d2a-cb8b-4cc4-991f-e2fe056a01fe",
          "name": "Get_link_referrers_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/referrers?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the pages referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b06a9f1b-025d-4ad0-a0e4-55a4ad05d4c3"
            }
          ]
        },
        {
          "id": "4c0bbd4b-0319-45a6-84db-e96cae2e3633",
          "name": "Get_link_shares_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/shares?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about a shares of a single link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b3a7d10-c312-4344-95c9-888c7b714151"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "af935d9d-11e1-47a7-bf81-2cbf7b65a297",
          "name": "Get_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/info?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to return the page title for a given bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "082df351-f734-4b89-98c8-7b47275513cd"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "28e485bb-8d6c-4bb9-99da-ae8013ac99ea",
          "name": "Get_user_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/info?format=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "393f8c0d-50ff-4b87-89ee-b59bd1563274"
            }
          ]
        },
        {
          "id": "f543323d-9d28-4a44-a391-69eb7b36f89f",
          "name": "Get_user_link_history_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/link_history?created_after=%7B%7D&created_before=%7B%7D&format=%7B%7D&limit=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5151bfaa-85ff-4e6d-8982-00bf57accd41"
            }
          ]
        },
        {
          "id": "6e4b2e08-2386-43f0-a8b8-9acc38ca7a56",
          "name": "Get_user_popular_links_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/popular_links?format=%7B%7D&limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's most-clicked bitly links (ordered by number of clicks) in a given time period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e81f3cfd-1ecf-4d92-8b4c-051ede28398d"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "483a8386-c858-4133-afbe-07b8c6a22002",
          "name": "Get_realtime_search_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/search?cities=%7B%7D&domain=%7B%7D&format=%7B%7D&lang=%7B%7D&limit=%7B%7D&offset=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search links receiving clicks across bitly by content, language, location, and more."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ab47a06-ad2d-4fa1-be55-3ffb6b762456"
            }
          ]
        }
      ]
    }
  ]
}