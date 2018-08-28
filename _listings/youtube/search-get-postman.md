{
  "info": {
    "name": "Youtube Get Search",
    "_postman_id": "740c3b50-f66c-4ae5-923f-3752542b52d8",
    "description": "Returns a collection of search results that match the query parameters specified in the API request. By default, a search result set identifies matching video, channel, and playlist resources, but you can also configure queries to only retrieve a specific type of resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "search",
      "item": [
        {
          "id": "80b7916a-6045-4272-834e-85672bb5c4db",
          "name": "getSearch",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/search?channelId=%7B%7D&channelType=%7B%7D&eventType=%7B%7D&forContentOwner=%7B%7D&forDeveloper=%7B%7D&forMine=%7B%7D&location=%7B%7D&locationRadius=%7B%7D&maxResults=%7B%7D&onBehalfOfContentOwner=%7B%7D&order=%7B%7D&pageToken=%7B%7D&part=%7B%7D&publishedAfter=%7B%7D&publishedBefore=%7B%7D&q=%7B%7D&regionCode=%7B%7D&relatedToVideoId=%7B%7D&relevanceLanguage=%7B%7D&safeSearch=%7B%7D&topicId=%7B%7D&type=%7B%7D&videoCaption=%7B%7D&videoCategoryId=%7B%7D&videoDefinition=%7B%7D&videoDimension=%7B%7D&videoDuration=%7B%7D&videoEmbeddable=%7B%7D&videoLicense=%7B%7D&videoSyndicated=%7B%7D&videoType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of search results that match the query parameters specified in the API request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f18ddef2-f213-46f9-b071-0c47087bc6fd"
            }
          ]
        }
      ]
    }
  ]
}