swagger: "2.0"
x-collection-name: Spotify
x-complete: 1
info:
  title: Spotify
  description: our-web-api-lets-your-applications-fetch-data-from-the-spotify-music-catalog-and-manage-users-playlists-and-saved-music--based-on-simple-rest-principles-our-web-api-endpoints-return-metadata-in-json-format-about-artists-albums-and-tracks-directly-from-the-spotify-catalogue--the-api-also-provides-access-to-userrelated-data-such-as-playlists-and-music-saved-in-a-your-music-library-subject-to-users-authorization-
  version: v1
host: api.spotify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Search
      description: '[Search for an Item](https://developer.spotify.com/web-api/search-item/)'
      operationId: search-for-an-itemhttpsdeveloperspotifycomwebapisearchitem
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: offset
        description: The index of the first item to return
      - in: query
        name: q
        description: The search querys keywords (and optional field filters)
      - in: query
        name: type
        description: A comma-separated list of item types to search across
      responses:
        200:
          description: OK
      tags:
      - Music
      - Search