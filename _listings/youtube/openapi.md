swagger: "2.0"
x-collection-name: YouTube
x-complete: 1
info:
  title: YouTube
  description: youtube-allows-users-to-upload-view-rate-share-add-to-favorites-report-comment-on-videos-and-subscribe-to-other-users--it-offers-a-wide-variety-of-usergenerated-and-corporate-media-videos--available-content-includes-video-clips-tv-show-clips-music-videos-short-and-documentary-films-audio-recordings-movie-trailers-live-streams-and-other-content-such-as-video-blogging-short-original-videos-and-educational-videos--most-of-the-content-on-youtube-is-uploaded-by-individuals-but-media-corporations-including-cbs-the-bbc-vevo-and-hulu-offer-some-of-their-material-via-youtube-as-part-of-the-youtube-partnership-program--unregistered-users-can-only-watch-videos-on-the-site-while-registered-users-are-permitted-to-upload-an-unlimited-number-of-videos-and-add-comments-to-videos-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Get Search
      description: Returns a collection of search results that match the query parameters
        specified in the API request. By default, a search result set identifies matching
        video, channel, and playlist resources, but you can also configure queries
        to only retrieve a specific type of resource.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter indicates that the API response should
          only contain resources created by the channel
      - in: query
        name: channelType
        description: The channelType parameter lets you restrict a search to a particular
          type of channel
      - in: query
        name: eventType
        description: The eventType parameter restricts a search to broadcast events
      - in: query
        name: forContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: forDeveloper
        description: The forDeveloper parameter restricts the search to only retrieve
          videos uploaded via the developers application or website
      - in: query
        name: forMine
        description: The forMine parameter restricts the search to only retrieve videos
          owned by the authenticated user
      - in: query
        name: location
        description: The location parameter, in conjunction with the locationRadius
          parameter, defines a circular geographic area and also restricts a search
          to videos that specify, in their metadata, a geographic location that falls
          within that area
      - in: query
        name: locationRadius
        description: The locationRadius parameter, in conjunction with the location
          parameter, defines a circular geographic area
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: order
        description: The order parameter specifies the method that will be used to
          order resources in the API response
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more search resource properties that the API response will include
      - in: query
        name: publishedAfter
        description: The publishedAfter parameter indicates that the API response
          should only contain resources created after the specified time
      - in: query
        name: publishedBefore
        description: The publishedBefore parameter indicates that the API response
          should only contain resources created before the specified time
      - in: query
        name: q
        description: The q parameter specifies the query term to search for
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return search results
          for the specified country
      - in: query
        name: relatedToVideoId
        description: The relatedToVideoId parameter retrieves a list of videos that
          are related to the video that the parameter value identifies
      - in: query
        name: relevanceLanguage
        description: The relevanceLanguage parameter instructs the API to return search
          results that are most relevant to the specified language
      - in: query
        name: safeSearch
        description: The safeSearch parameter indicates whether the search results
          should include restricted content as well as standard content
      - in: query
        name: topicId
        description: The topicId parameter indicates that the API response should
          only contain resources associated with the specified topic
      - in: query
        name: type
        description: The type parameter restricts a search query to only retrieve
          a particular type of resource
      - in: query
        name: videoCaption
        description: The videoCaption parameter indicates whether the API should filter
          video search results based on whether they have captions
      - in: query
        name: videoCategoryId
        description: The videoCategoryId parameter filters video search results based
          on their category
      - in: query
        name: videoDefinition
        description: The videoDefinition parameter lets you restrict a search to only
          include either high definition (HD) or standard definition (SD) videos
      - in: query
        name: videoDimension
        description: The videoDimension parameter lets you restrict a search to only
          retrieve 2D or 3D videos
      - in: query
        name: videoDuration
        description: The videoDuration parameter filters video search results based
          on their duration
      - in: query
        name: videoEmbeddable
        description: The videoEmbeddable parameter lets you to restrict a search to
          only videos that can be embedded into a webpage
      - in: query
        name: videoLicense
        description: The videoLicense parameter filters search results to only include
          videos with a particular license
      - in: query
        name: videoSyndicated
        description: The videoSyndicated parameter lets you to restrict a search to
          only videos that can be played outside youtube
      - in: query
        name: videoType
        description: The videoType parameter lets you restrict a search to a particular
          type of videos
      responses:
        200:
          description: OK
      tags:
      - Search