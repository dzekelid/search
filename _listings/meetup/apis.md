---
name: Meetup
x-slug: meetup
description: Find Meetups so you can do more of what matters to you. Or create your
  own group and meet people near you who share your interests.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
x-kinRank: "9"
x-alexaRank: "917"
tags: Search
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/apis.md
specificationVersion: "0.14"
apis:
- name: Meetup - Find Events
  x-api-slug: findevents-get
  description: Returns list of upcoming events based on location
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findevents-get-openapi.md
- name: Meetup - Find Upcoming Events
  x-api-slug: findupcoming-events-get
  description: Returns a list of upcoming events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findupcoming-events-get-openapi.md
- name: Meetup - Find Groups
  x-api-slug: findgroups-get
  description: Text, location, category and friend-based group searches
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findgroups-get-openapi.md
- name: Meetup - Find Venues
  x-api-slug: findvenues-get
  description: Returns list of venues based on location
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findvenues-get-openapi.md
- name: Meetup - Group Profile search
  x-api-slug: findurlnamemembers-get
  description: |-
    Find group member profiles by name.
    Member's who very recently joined or left the group may not be immediately searchable
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findurlnamemembers-get-openapi.md
- name: Meetup - Find locations
  x-api-slug: findlocations-get
  description: Provides a query interface for finding known locations
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findlocations-get-openapi.md
- name: Meetup - Topic Categories
  x-api-slug: findtopic-categories-get
  description: Returns a list high level topic categories
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findtopic-categories-get-openapi.md
- name: Meetup - Find Topics
  x-api-slug: findtopics-get
  description: Find topics by name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/meetup/findtopics-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://medium.api.gallery.streamdata.io
- type: x-api-stack
  url: http://meetup.stack.network
- type: x-base
  url: http://api.meetup.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/meetup
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-email
  url: privacy@meetup.com
- type: x-email
  url: abuse@meetup.com
- type: x-email
  url: api_license@meetup.com
- type: x-email
  url: arbitration-opt-out@meetup.com
- type: x-email
  url: legal@meetup.com
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-twitter
  url: https://twitter.com/Meetup
- type: x-website
  url: http://meetup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---