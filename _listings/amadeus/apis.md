---
name: Amadeus
x-slug: amadeus
description: Amadeus travel technology helps businesses connect to the global travel
  ecosystem, manage operations more effectively and serve travellers better than ever
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
x-kinRank: "8"
x-alexaRank: "4309"
tags: Search
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/apis.md
specificationVersion: "0.14"
apis:
- name: Amadeus - Get Cars Search Airport
  x-api-slug: carssearchairport-get
  description: "With this API you can find out the price and type of car, for all
    car rental providers, near a specified airport.\n\nYou can quickly see the locations
    of car providers near a given airport, and what cars are available to rent, and
    at what prices. This API is based on our car pricing service that gets live availability
    from car providers, and is used to power a variety of airline and travel agency
    websites.\n           \nResults are validated from car providers, and thus response
    times may take up to 10 seconds (response times are typically about 5s), and the
    number of concurrent calls is throttled per user to avoid flooding our provider's
    systems. However, this means the final result is guaranteed to be live and accurate.\n\nThe
    configuration of this API allows search for car rentals in the rental location
    where the car is picked up (at the start of the rental), is the same as the one
    where it will be dropped off."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/carssearchairport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/carssearchairport-get-openapi.md
- name: Amadeus - Get Cars Search
  x-api-slug: carssearchcircle-get
  description: "With this API you can find out the price and type of car, for all
    car rental providers, in a specified geographical location.\n\nYou can quickly
    see the locations of car providers near a given point, and what cars are available
    to rent, and at what prices. This API is based on our car pricing service that
    gets live availability from car providers, and is used to power a variety of airline
    and travel agency websites.\n           \nResults are validated from car providers,
    and thus response times may take up to 10 seconds (response times are typically
    about 5s), and the number of concurrent calls is throttled per user to avoid flooding
    our provider's systems. However, this means the final result is guaranteed to
    be live and accurate.\n\nThe configuration of this API allows search for car rentals
    in the rental location where the car is picked up (at the start of the rental),
    is the same as the one where it will be dropped off."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/carssearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/carssearchcircle-get-openapi.md
- name: Amadeus - Get Flights Affiliate Search
  x-api-slug: flightsaffiliatesearch-get
  description: "The Flight Affiliate Search API combines Amadeus' flight search technology
    with Travel Audience's Connect API partners to provide a unique flight search,
    where all results come with deep-links to book the flight at a partner's website.
    The API will let you easily provide the traveler with a path to book flights from
    your application.\nTravel Audience Connect partners include\n\n  CityJet, Air
    Europa and TAP in Western Europe,\n  Ural Airlines in Russia, \n  Avianca Brazil
    \ and\n  JAL in East Asia\n\n\nOnly Travel Audience Connect partner airlines are
    searched. For an up-to-date list of routes, see the route maps on each partners
    respective websites above. You can earn commission using the deep links provided
    in the search results if you sign up for an account at connect.travelaudience.com."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightsaffiliatesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightsaffiliatesearch-get-openapi.md
- name: Amadeus - Get Flights Extensive Search
  x-api-slug: flightsextensivesearch-get
  description: |-
    The Extensive Flight Search allows you to find the prices of one-way or return flights between two airports over a large number of dates, and for a large variety of stay durations. The search doesn't return exact itineraries, but rather tells you the best price for a flight on a given day, for a stay of a given duration.

    The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

    That said, a price graph like this provides a powerful bargin shopping tool - allowing travelers with flexible itineraries to identify days on which they can get the cheapest flights to their destinations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightsextensivesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightsextensivesearch-get-openapi.md
- name: Amadeus - Get Flights Inspiration Search
  x-api-slug: flightsinspirationsearch-get
  description: |-
    The Inspiration Flight Search allows you to find the prices of one-way and return flights from an origin city without necessarily having a destination, or even a flight date, in mind. The search doesn't return a distinct set of price options, but rather, can tell you the price of flying from a given city to some destination, for a trip of a given duration, that falls within a given date range.

    The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

    Despite this limitation don't underestimate the power of this API. Thanks to its quick response speed you can easily pair it with other APIs to provide a low fare and inspiration for any destination. For example, you can could combine it with a event search API and suggest a total price to see go and see an concert or a game in a selection of cities.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightsinspirationsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightsinspirationsearch-get-openapi.md
- name: Amadeus - Get Flights Low Fare Search
  x-api-slug: flightslowfaresearch-get
  description: "This is the low fare search engine Amadeus uses to retrieve the best
    price for flights, based on our latest Master Pricer Travel Board technology.
    This document describes how to make a low fare search and how to handle the returned
    messages.\n\nThe message is composed of multiple results for given request. A
    result is defined by a unique combination of price, tax, passenger type, fare
    type, cabin, and availability for each requested segment. \n\nA result is then
    composed of single or multiple itineraries. Each itinerary is composed of an outbound
    leg, and, if a return date was specified, an inbound leg. Each leg is composed
    of a list of one or more flights, that the traveller will be required to take
    in order to get from the origin airport to the destination airport."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightslowfaresearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/flightslowfaresearch-get-openapi.md
- name: Amadeus - Get Hotels Search Airport
  x-api-slug: hotelssearchairport-get
  description: |-
    A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.

    This API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/hotelssearchairport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/hotelssearchairport-get-openapi.md
- name: Amadeus - Get Hotels Search Box
  x-api-slug: hotelssearchbox-get
  description: "A fast Hotel shopping API to see which hotels are available in a given
    area, on a given day and displays their lowest prices. With this API you can find
    out the price of the cheapest daily rate for all hotels within a specified geographical
    region.\n\nThis API allows you to quickly see the hotel locations in a region,
    and what prices in that area look like,  as well as the check-in and check-out
    dates, and get a list of up to 140 properties (names, codes, image, amenities)
    with their locations and rates. Optional parameters such as currency and maximum
    rates, amenities or hotel chain codes are also available and can be used to narrow
    down the results. More optional parameters such as show_sold_out & rooms can be
    used to show sold out rooms and all available rooms.\n            \nThe API is
    based on our high-speed hotel pricing cache, which is also used to power the Amadeus
    Hotel Search Engine application. Results are returned very quickly, response times
    are generally under 2s. Our cache has great global coverage and is constantly
    refreshed with the latest prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/hotelssearchbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/hotelssearchbox-get-openapi.md
- name: Amadeus - Get Hotels Search Circle
  x-api-slug: hotelssearchcircle-get
  description: "A fast Hotel shopping API to see which hotels are available in a given
    area, on a given day and displays their lowest prices. With this API you can find
    out the price of the cheapest daily rate for all hotels within a specified radius
    of a point.\n\nThis API allows you to quickly see the hotel locations in a region,
    and what prices in that area look like,  as well as the check-in and check-out
    dates, and get list of up to 140 properties (names, codes, image, amenities) with
    their locations and rates. Optional parameters such as currency and maximum rates,
    amenities or hotel chain codes are also available and can be used to narrow down
    the results. More optional parameters such as show_sold_out & rooms can be used
    to show sold out rooms and all available rooms. \n\nThe API is based on our high-speed
    hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine
    application. Results are returned very quickly, response times are generally under
    2s. Our cache has great global coverage and is constantly refreshed with the latest
    prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/hotelssearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/hotelssearchcircle-get-openapi.md
- name: Amadeus - Get Points Of Interest Yapq Search Circle
  x-api-slug: pointsofinterestyapqsearchcircle-get
  description: "Amadeus has partnered with YapQ to bring you point of interest APIs
    with the goal of offering you unbiased ratings of landmarks and tourist attractions.
    YapQ rates places according to their interest on social media and provides Wikipedia
    content and Geonames ID at a given location. \nYapQ's service indexes millions
    of points around the world, and provides content in 12 different languages. This
    allows you to ensure you catch the must-see sights at a specific YapQ supported
    location.\nEach point of interest comes with links to content, grading information,
    location and directions to help make discovering your destination easy and fun.\nThis
    service is still under active development, and the response format may change
    without warning. We'd be interested in your feedback - send us an email."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/pointsofinterestyapqsearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/pointsofinterestyapqsearchcircle-get-openapi.md
- name: Amadeus - Get Points Of Interest Yapq Search Text
  x-api-slug: pointsofinterestyapqsearchtext-get
  description: "Amadeus has partnered with YapQ to bring you point of interest APIs
    with the goal of offering you unbiased ratings of landmarks and tourist attractions.
    YapQ rates these points according to their interest on social media and provides
    Wikipedia content and Geonames ID in a given city. \nYapQ's service indexes millions
    of points around the world, and provides content in 12 different languages. This
    allows you to ensure you catch the must-see sights in a YapQ supported city.\nEach
    point of interest comes with links to content, grading information, location and
    directions to help make discovering your destination easy and fun.\nThis service
    is still under active development, and the response format may change without
    warning. We'd be interested in your feedback - send us an email."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/pointsofinterestyapqsearchtext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/pointsofinterestyapqsearchtext-get-openapi.md
- name: Amadeus - Get Trains Extensive Search
  x-api-slug: trainsextensivesearch-get
  description: "This API allows you to search trains availability and prices for a
    single day or date range. It's based on our Rail Instant Search technology, providing
    you with immediate results from our rail search cache.\n\nThis API has content
    from SNCF (French trains).\n            \nThe content is also restricted to single-leg
    trips - where a single train takes you directly from the origin to the destination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/trainsextensivesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/trainsextensivesearch-get-openapi.md
- name: Amadeus - Get Trains Schedule Search
  x-api-slug: trainsschedulesearch-get
  description: |-
    This API allows you to find all the possible destinations in the Rail Instant Search cache (used by Extensive Search above) from a given origin station on a given day. You can use this to help build network maps, journey planners or provide inspiration for rail travel.

    This API has continuous content from SNCF.
    All the options returned are single-leg trips - where a single train takes you directly from the origin to the destination. In general, only departure dates up to 90 days in the future are supported

    Currently agglomeration stations are not supported
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/trainsschedulesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/amadeus/trainsschedulesearch-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://amadeus.api.gallery.streamdata.io
- type: x-api-stack
  url: http://amadeus.stack.network
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