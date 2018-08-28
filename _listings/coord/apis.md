---
name: Coord
x-slug: coord
description: Coord is a mobility company that creates seamless mobility and self-driving
  experiences today through deep integrations. The company offers bike-share API,
  Curbs API, Tolls API, Routing API and etc.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
x-kinRank: "7"
x-alexaRank: "1035226"
tags: Search
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/coord/apis.md
specificationVersion: "0.14"
apis:
- name: Bike Share API - Get bike locations in the requested search area, as a GeoJSON
    FeatureCollection.
  x-api-slug: location-get
  description: |-
    Get a list of locations given the input parameters. Specify a search area by radius around
    a latitude and longitude, as well as any filter for specific systems. Each location will
    be a GeoJSON Feature, and aggregated into a GeoJSON FeatureCollection.

    ### Example

    #### Request:
    `curl -G "https://api.coord.co/v1/bike/location?latitude=40.742868&longitude=-73.989186&radius_km=0.25&access_key="`

    #### Response:
    ```
    {
      "features": [
        {
          "geometry": {
            "coordinates": [
              -73.98918628692627,
              40.74286877312112
            ],
            "type": "Point"
          },
          "id": "CitiBike-3641",
          "properties": {
            "is_renting": true,
            "is_returning": true,
            "last_reported": "2018-05-17T15:39:24.000Z",
            "lat": 40.74286877312112,
            "location_id": "3641",
            "location_type": "bike_station_dock",
            "lon": -73.98918628692627,
            "name": "Broadway & W 25 St",
            "num_bikes_available": 53,
            "num_docks_available": 1,
            "region_id": "71",
            "system_id": "CitiBike"
          },
          "type": "Feature"
        },
        {
          "geometry": {
            "coordinates": [
              -73.99144871,
              40.74395411
            ],
            "type": "Point"
          },
          "id": "CitiBike-466",
          "properties": {
            "is_renting": true,
            "is_returning": true,
            "last_reported": "2018-05-17T15:32:40.000Z",
            "lat": 40.74395411,
            "location_id": "466",
            "location_type": "bike_station_dock",
            "lon": -73.99144871,
            "name": "W 25 St & 6 Ave",
            "num_bikes_available": 35,
            "region_id": "71",
            "system_id": "CitiBike"
          },
          "type": "Feature"
        }
      ],
      "type": "FeatureCollection"
    }
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/bike
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/coord/location-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/coord/location-get-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/coord
- type: x-blog-rss
  url: https://medium.com/feed/coord
- type: x-openapi
  url: https://jsapi.apiary.io/apis/coordprodsearchtolls.source
- type: x-api-gallery
  url: http://convertapi.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coord.stack.network
- type: x-developer
  url: https://coord.co/docs/
- type: x-pricing
  url: https://coord.co/#pricing
- type: x-twitter
  url: https://twitter.com/coordcity
- type: x-website
  url: https://coord.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---