---
name: Amadeus
description: Amadeus travel technology helps businesses connect to the global travel
  ecosystem, manage operations more effectively and serve travellers better than ever
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
x-kinRank: "8"
x-alexaRank: "4309"
tags:
- Travel
- Transportation
- Technology
- Marketplace
- Hotel
- Airlines
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/apis.yaml
specificationVersion: "0.14"
apis:
- name: Amadeus
  description: Amadeus travel technology helps businesses connect to the global travel
    ecosystem, manage operations more effectively and serve travellers better than
    ever
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: ""
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/travel-intelligence-top-searches-get.md
- name: Amadeus Get Flights Inspiration Search
  description: |-
    The Inspiration Flight Search allows you to find the prices of one-way and return flights from an origin city without necessarily having a destination, or even a flight date, in mind. The search doesn't return a distinct set of price options, but rather, can tell you the price of flying from a given city to some destination, for a trip of a given duration, that falls within a given date range.

    The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

    Despite this limitation don't underestimate the power of this API. Thanks to its quick response speed you can easily pair it with other APIs to provide a low fare and inspiration for any destination. For example, you can could combine it with a event search API and suggest a total price to see go and see an concert or a game in a selection of cities.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flights-inspiration-search-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flights-inspiration-search-get-postman.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/amadeus
- type: x-documentation
  url: https://sandbox.amadeus.com/api-catalog
- type: x-github
  url: https://github.com/AmadeusITGroup
- type: x-privacy-policy
  url: http://www.amadeus.com/web/amadeus/en_1A-corporate/Amadeus-Home/Amadeus_IT_Group_SA-Legal-notices-2014/1319560218660-Page-AMAD_Detail_PopUp_Ppal?assetid=1319607040997&assettype=DataProtection_C
- type: x-sandbox
  url: https://sandbox.amadeus.com
- type: x-terms-of-service
  url: http://www.amadeus.com/web/amadeus/en_1A-corporate/Amadeus-Home/Amadeus_IT_Group_SA-Legal-notices-2014/1319560218660-Page-AMAD_Detail_PopUp_Ppal?assetid=1319607040997&assettype=DataProtection_C
- type: x-twitter
  url: https://twitter.com/amadeusinnov
- type: x-website
  url: https://amadeus.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/amadeus
- type: x-documentation
  url: https://sandbox.amadeus.com/api-catalog
- type: x-github
  url: https://github.com/AmadeusITGroup
- type: x-privacy-policy
  url: http://www.amadeus.com/web/amadeus/en_1A-corporate/Amadeus-Home/Amadeus_IT_Group_SA-Legal-notices-2014/1319560218660-Page-AMAD_Detail_PopUp_Ppal?assetid=1319607040997&assettype=DataProtection_C
- type: x-sandbox
  url: https://sandbox.amadeus.com
- type: x-terms-of-service
  url: http://www.amadeus.com/web/amadeus/en_1A-corporate/Amadeus-Home/Amadeus_IT_Group_SA-Legal-notices-2014/1319560218660-Page-AMAD_Detail_PopUp_Ppal?assetid=1319607040997&assettype=DataProtection_C
- type: x-twitter
  url: https://twitter.com/amadeusinnov
- type: x-website
  url: https://amadeus.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---