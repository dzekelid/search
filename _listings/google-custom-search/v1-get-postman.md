{
  "info": {
    "name": "Google Custom Search JSON/Atom API Search",
    "_postman_id": "94a392f9-e4f8-4a75-af1e-7b7d582a64c3",
    "description": "Returns metadata about the search performed, metadata about the custom search engine used for the search, and the search results.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "search",
      "item": [
        {
          "id": "5cb60a26-a50f-4f38-817b-7c7eb5e0f0e8",
          "name": "search.cse.list",
          "request": {
            "url": "http://www.googleapis.com/customsearch/v1?c2coff=%7B%7D&cr=%7B%7D&cref=%7B%7D&cx=%7B%7D&dateRestrict=%7B%7D&exactTerms=%7B%7D&excludeTerms=%7B%7D&fileType=%7B%7D&filter=%7B%7D&gl=%7B%7D&googlehost=%7B%7D&highRange=%7B%7D&hl=%7B%7D&hq=%7B%7D&imgColorType=%7B%7D&imgDominantColor=%7B%7D&imgSize=%7B%7D&imgType=%7B%7D&linkSite=%7B%7D&lowRange=%7B%7D&lr=%7B%7D&num=%7B%7D&orTerms=%7B%7D&q=%7B%7D&relatedSite=%7B%7D&rights=%7B%7D&safe=%7B%7D&searchType=%7B%7D&siteSearch=%7B%7D&siteSearchFilter=%7B%7D&sort=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metadata about the search performed, metadata about the custom search engine used for the search, and the search results"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12914b37-6a8d-454f-8fb4-e7ffb4e32682"
            }
          ]
        }
      ]
    }
  ]
}