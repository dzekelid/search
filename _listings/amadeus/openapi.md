swagger: "2.0"
x-collection-name: Amadeus
x-complete: 1
info:
  title: Amadeus
  description: amadeus-api-is-a-toolkit-designed-for-travel-agencies-who-want-to-develop-their-own-travel-products-rather-than-using-offtheshelf-solutions--with-this-tool-you-can-build-your-very-own-customised-applications-that-link-in-a-stable-and-secure-dialogue-with-our-global-distribution-system-gds-
  contact:
    name: Amadeus Innovation and Research
    url: https://sandbox.amadeus.com
  version: 1.0.0
host: api.sandbox.amadeus.com
basePath: /v1.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cars/search-airport:
    get:
      summary: Get Cars Search Airport
      description: "With this API you can find out the price and type of car, for
        all car rental providers, near a specified airport.\n\nYou can quickly see
        the locations of car providers near a given airport, and what cars are available
        to rent, and at what prices. This API is based on our car pricing service
        that gets live availability from car providers, and is used to power a variety
        of airline and travel agency websites.\n           \nResults are validated
        from car providers, and thus response times may take up to 10 seconds (response
        times are typically about 5s), and the number of concurrent calls is throttled
        per user to avoid flooding our provider's systems. However, this means the
        final result is guaranteed to be live and accurate.\n\nThe configuration of
        this API allows search for car rentals in the rental location where the car
        is picked up (at the start of the rental), is the same as the one where it
        will be dropped off."
      operationId: getCarsSearchAirport
      x-api-path-slug: carssearchairport-get
      parameters:
      - in: query
        name: currency
        description: The preferred currency to use when displaying prices and rates
          related to the car rental
      - in: query
        name: drop_off
        description: Date at which the car rental will end and the car will be returned
          to the rental location
      - in: query
        name: lang
        description: The preferred language of the content related to each car rental
      - in: query
        name: location
        description: The IATA code of the airport at which the car will be rented
      - in: query
        name: pick_up
        description: Date on which the car rental will be collected from the car rental
          location
      - in: query
        name: provider
        description: 2 character car rental provider code
      - in: query
        name: rate_class
        description: Allows to request specific rate types
      - in: query
        name: rate_filter
        description: Defines the types of rates to be returned in the output
      - in: query
        name: rate_plan
        description: Qualifies the rate depending on the pickup date and the rental
          duration
      - in: query
        name: vehicle
        description: Specifies the type of vehicle to be rented
      responses:
        200:
          description: OK
      tags:
      - Cars
      - Search
      - Airport
  /cars/search-circle:
    get:
      summary: Get Cars Search
      description: "With this API you can find out the price and type of car, for
        all car rental providers, in a specified geographical location.\n\nYou can
        quickly see the locations of car providers near a given point, and what cars
        are available to rent, and at what prices. This API is based on our car pricing
        service that gets live availability from car providers, and is used to power
        a variety of airline and travel agency websites.\n           \nResults are
        validated from car providers, and thus response times may take up to 10 seconds
        (response times are typically about 5s), and the number of concurrent calls
        is throttled per user to avoid flooding our provider's systems. However, this
        means the final result is guaranteed to be live and accurate.\n\nThe configuration
        of this API allows search for car rentals in the rental location where the
        car is picked up (at the start of the rental), is the same as the one where
        it will be dropped off."
      operationId: getCarsSearchCircle
      x-api-path-slug: carssearchcircle-get
      parameters:
      - in: query
        name: currency
        description: The preferred currency to use when displaying prices and rates
          related to the car rental
      - in: query
        name: drop_off
        description: Date at which the car rental will end and the car will be returned
          to the rental location
      - in: query
        name: lang
        description: The preferred language of the content related to each car rental
      - in: query
        name: latitude
        description: Latitude of the center of the search
      - in: query
        name: longitude
        description: Longitude of the center of the search
      - in: query
        name: pick_up
        description: Date on which the car rental will be collected from the car rental
          location
      - in: query
        name: provider
        description: 2 character car rental provider code
      - in: query
        name: radius
        description: Radius around the center to look for hotels in kilometers (km)
      - in: query
        name: rate_class
        description: Allows to request specific rate types
      - in: query
        name: rate_filter
        description: Defines the types of rates to be returned in the output
      - in: query
        name: rate_plan
        description: Qualifies the rate depending on the pickup date and the rental
          duration
      - in: query
        name: vehicle
        description: Specifies the type of vehicle to be rented
      responses:
        200:
          description: OK
      tags:
      - Cars
      - Search
      - Circle
  /flights/affiliate-search:
    get:
      summary: Get Flights Affiliate Search
      description: "The Flight Affiliate Search API combines Amadeus' flight search
        technology with Travel Audience's Connect API partners to provide a unique
        flight search, where all results come with deep-links to book the flight at
        a partner's website. The API will let you easily provide the traveler with
        a path to book flights from your application.\nTravel Audience Connect partners
        include\n\n  CityJet, Air Europa and TAP in Western Europe,\n  Ural Airlines
        in Russia, \n  Avianca Brazil  and\n  JAL in East Asia\n\n\nOnly Travel Audience
        Connect partner airlines are searched. For an up-to-date list of routes, see
        the route maps on each partners respective websites above. You can earn commission
        using the deep links provided in the search results if you sign up for an
        account at connect.travelaudience.com."
      operationId: getFlightsAffiliateSearch
      x-api-path-slug: flightsaffiliatesearch-get
      parameters:
      - in: query
        name: adults
        description: The number of adult (age 12 and over) passengers traveling on
          this flight
      - in: query
        name: children
        description: The number of child (younger than age 12 on date of departure)
          passengers traveling on this flight who will each have their own separate
          seat
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: departure_date
        description: The date on which the traveler will depart from the origin to
          go to the destination
      - in: query
        name: destination
        description: IATA code of the city to which the traveler is going
      - in: query
        name: exclude_merchants
        description: If specified, no results will include any flights where any of
          these airlines is the marketing carrier
      - in: query
        name: include_merchants
        description: If specified, all results will include at least one flight where
          one or more of these airlines is the marketing carrier
      - in: query
        name: infants
        description: The number of infant (younger than age 2 on date of departure)
          passengers traveling on this flight
      - in: query
        name: max_price
        description: Maximum price of trips to find in the result set, in USD (US
          dollars) unless some other currency code is specified
      - in: query
        name: mobile
        description: Setting this to true will show mobile web deeplinks
      - in: query
        name: origin
        description: City code from which the traveler will depart
      - in: query
        name: return_date
        description: The date on which the traveler will depart from the destination
          to return to the origin
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Flights
      - Affiliate
      - Search
  /flights/extensive-search:
    get:
      summary: Get Flights Extensive Search
      description: |-
        The Extensive Flight Search allows you to find the prices of one-way or return flights between two airports over a large number of dates, and for a large variety of stay durations. The search doesn't return exact itineraries, but rather tells you the best price for a flight on a given day, for a stay of a given duration.

        The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

        That said, a price graph like this provides a powerful bargin shopping tool - allowing travelers with flexible itineraries to identify days on which they can get the cheapest flights to their destinations.
      operationId: getFlightsExtensiveSearch
      x-api-path-slug: flightsextensivesearch-get
      parameters:
      - in: query
        name: aggregation_mode
        description: Specifies the granularity of results to be found
      - in: query
        name: departure_date
        description: Range of dates between which the traveler could depart
      - in: query
        name: destination
        description: IATA code of the city to which the traveler is going
      - in: query
        name: direct
        description: Limit the search to results that do not require the passenger
          to change plane?
      - in: query
        name: duration
        description: The allowed duration or range of durations of the trip, in days
      - in: query
        name: max_price
        description: Maximum price of trips to find in the result set, in the currency
          specified for this origin and destination pair in the cache contents spreadsheet
      - in: query
        name: one-way
        description: When set to true, the query will be for a single trip from the
          origin to the destination
      - in: query
        name: origin
        description: IATA code of the city from which the traveler will depart
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Flights
      - Extensive
      - Search
  /flights/inspiration-search:
    get:
      summary: Get Flights Inspiration Search
      description: |-
        The Inspiration Flight Search allows you to find the prices of one-way and return flights from an origin city without necessarily having a destination, or even a flight date, in mind. The search doesn't return a distinct set of price options, but rather, can tell you the price of flying from a given city to some destination, for a trip of a given duration, that falls within a given date range.

        The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

        Despite this limitation don't underestimate the power of this API. Thanks to its quick response speed you can easily pair it with other APIs to provide a low fare and inspiration for any destination. For example, you can could combine it with a event search API and suggest a total price to see go and see an concert or a game in a selection of cities.
      operationId: getFlightsInspirationSearch
      x-api-path-slug: flightsinspirationsearch-get
      parameters:
      - in: query
        name: aggregation_mode
        description: Specifies the granularity of results to be found
      - in: query
        name: departure_date
        description: Range of dates between which the traveler could depart
      - in: query
        name: destination
        description: IATA code of the city to which the traveler is going
      - in: query
        name: direct
        description: Limit the search to results that do not require the passenger
          to change plane?
      - in: query
        name: duration
        description: The allowed duration or range of durations of the trip, in days
      - in: query
        name: max_price
        description: Maximum price of trips to find in the result set, in the currency
          specified for this origin and destination pair in the cache contents spreadsheet
      - in: query
        name: one-way
        description: When set to true, the query will be for a single trip from the
          origin to the destination
      - in: query
        name: origin
        description: IATA code of the city from which the traveler will depart
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Flights
      - Inspiration
      - Search
  /flights/low-fare-search:
    get:
      summary: Get Flights Low Fare Search
      description: "This is the low fare search engine Amadeus uses to retrieve the
        best price for flights, based on our latest Master Pricer Travel Board technology.
        This document describes how to make a low fare search and how to handle the
        returned messages.\n\nThe message is composed of multiple results for given
        request. A result is defined by a unique combination of price, tax, passenger
        type, fare type, cabin, and availability for each requested segment. \n\nA
        result is then composed of single or multiple itineraries. Each itinerary
        is composed of an outbound leg, and, if a return date was specified, an inbound
        leg. Each leg is composed of a list of one or more flights, that the traveller
        will be required to take in order to get from the origin airport to the destination
        airport."
      operationId: getFlightsLowFareSearch
      x-api-path-slug: flightslowfaresearch-get
      parameters:
      - in: query
        name: adults
        description: The number of adult (age 12 and over) passengers traveling on
          this flight
      - in: query
        name: arrive_by
        description: The datetime by which the outbound flight should arrive, based
          on local time at the destination airport
      - in: query
        name: children
        description: The number of child (younger than age 12 on date of departure)
          passengers traveling on this flight who will each have their own separate
          seat
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: departure_date
        description: The date on which the traveler will depart from the origin to
          go to the destination
      - in: query
        name: destination
        description: IATA code of the city to which the traveler is going
      - in: query
        name: exclude_airlines
        description: If specified, no results will include any flights where any of
          these airlines is the marketing carrier
      - in: query
        name: include_airlines
        description: If specified, all results will include at least one flight where
          one or more of these airlines is the marketing carrier
      - in: query
        name: infants
        description: The number of infant (younger than age 2 on date of departure)
          passengers traveling on this flight
      - in: query
        name: max_price
        description: Maximum price of trips to find in the result set, in USD (US
          dollars) unless some other currency code is specified
      - in: query
        name: nonstop
        description: Setting this to true will find only flights that do not require
          the passenger to change from one flight to another
      - in: query
        name: number_of_results
        description: The number of results to display
      - in: query
        name: origin
        description: City code from which the traveler will depart
      - in: query
        name: return_by
        description: The time by which the inbound flight should arrive, based on
          local time at the airport specified as the origin parameter
      - in: query
        name: return_date
        description: The date on which the traveler will depart from the destination
          to return to the origin
      - in: query
        name: travel_class
        description: Searches for results where the majority of the itinerary flight
          time should be in a the specified cabin class or higher
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Flights
      - Low
      - Fare
      - Search
  /hotels/search-airport:
    get:
      summary: Get Hotels Search Airport
      description: |-
        A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.

        This API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.
      operationId: getHotelsSearchAirport
      x-api-path-slug: hotelssearchairport-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: amenity
        description: Hotel amenities filter to search narrow down hotels with certain
          amenities
      - in: query
        name: chain
        description: Narrows the hotel search to a given hotel provider
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: query
        name: location
        description: IATA airport code for hotel availability is required requested
      - in: query
        name: max_rate
        description: The maximum amount per night that any hotel in the shopping response
          should cost
      - in: query
        name: number_of_results
        description: The maximum number of hotels to return in the results set
      - in: query
        name: radius
        description: Radius around the center to look for hotels in kilometers (km)
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Search
      - Airport
  /hotels/search-box:
    get:
      summary: Get Hotels Search Box
      description: "A fast Hotel shopping API to see which hotels are available in
        a given area, on a given day and displays their lowest prices. With this API
        you can find out the price of the cheapest daily rate for all hotels within
        a specified geographical region.\n\nThis API allows you to quickly see the
        hotel locations in a region, and what prices in that area look like,  as well
        as the check-in and check-out dates, and get a list of up to 140 properties
        (names, codes, image, amenities) with their locations and rates. Optional
        parameters such as currency and maximum rates, amenities or hotel chain codes
        are also available and can be used to narrow down the results. More optional
        parameters such as show_sold_out & rooms can be used to show sold out rooms
        and all available rooms.\n            \nThe API is based on our high-speed
        hotel pricing cache, which is also used to power the Amadeus Hotel Search
        Engine application. Results are returned very quickly, response times are
        generally under 2s. Our cache has great global coverage and is constantly
        refreshed with the latest prices."
      operationId: getHotelsSearchBox
      x-api-path-slug: hotelssearchbox-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: amenity
        description: Hotel amenities filter to search narrow down hotels with certain
          amenities
      - in: query
        name: chain
        description: Narrows the hotel search to a given hotel provider
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: query
        name: max_rate
        description: The maximum amount per night that any hotel in the shopping response
          should cost
      - in: query
        name: north_east_corner
        description: The coordinates of the north-east corner of the search box
      - in: query
        name: number_of_results
        description: The maximum number of hotels to return in the results set
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      - in: query
        name: south_west_corner
        description: The coordinates of the south-west corner of the search box
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Search
      - Box
  /hotels/search-circle:
    get:
      summary: Get Hotels Search Circle
      description: "A fast Hotel shopping API to see which hotels are available in
        a given area, on a given day and displays their lowest prices. With this API
        you can find out the price of the cheapest daily rate for all hotels within
        a specified radius of a point.\n\nThis API allows you to quickly see the hotel
        locations in a region, and what prices in that area look like,  as well as
        the check-in and check-out dates, and get list of up to 140 properties (names,
        codes, image, amenities) with their locations and rates. Optional parameters
        such as currency and maximum rates, amenities or hotel chain codes are also
        available and can be used to narrow down the results. More optional parameters
        such as show_sold_out & rooms can be used to show sold out rooms and all available
        rooms. \n\nThe API is based on our high-speed hotel pricing cache, which is
        also used to power the Amadeus Hotel Search Engine application. Results are
        returned very quickly, response times are generally under 2s. Our cache has
        great global coverage and is constantly refreshed with the latest prices."
      operationId: getHotelsSearchCircle
      x-api-path-slug: hotelssearchcircle-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: amenity
        description: Hotel amenities filter to search narrow down hotels with certain
          amenities
      - in: query
        name: chain
        description: Narrows the hotel search to a given hotel provider
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: query
        name: latitude
        description: Latitude of the center of the search
      - in: query
        name: longitude
        description: Longitude of the center of the search
      - in: query
        name: max_rate
        description: The maximum amount per night that any hotel in the shopping response
          should cost
      - in: query
        name: number_of_results
        description: The maximum number of hotels to return in the results set
      - in: query
        name: radius
        description: Radius around the center to look for hotels in kilometers (km)
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Search
      - Circle
  /points-of-interest/yapq-search-circle:
    get:
      summary: Get Points Of Interest Yapq Search Circle
      description: "Amadeus has partnered with YapQ to bring you point of interest
        APIs with the goal of offering you unbiased ratings of landmarks and tourist
        attractions. YapQ rates places according to their interest on social media
        and provides Wikipedia content and Geonames ID at a given location. \nYapQ's
        service indexes millions of points around the world, and provides content
        in 12 different languages. This allows you to ensure you catch the must-see
        sights at a specific YapQ supported location.\nEach point of interest comes
        with links to content, grading information, location and directions to help
        make discovering your destination easy and fun.\nThis service is still under
        active development, and the response format may change without warning. We'd
        be interested in your feedback - send us an email."
      operationId: getPointsOfInterestYapqSearchCircle
      x-api-path-slug: pointsofinterestyapqsearchcircle-get
      parameters:
      - in: query
        name: category
        description: Filters the resulting points_of_interest to include only results
          which have a least one category containing the given provided word
      - in: query
        name: geonames
        description: Setting this to true includes only points of interest with a
          geonames ID
      - in: query
        name: image_size
        description: The size of the images youd like to see in the response
      - in: query
        name: lang
        description: The preferred language of the content related to each point of
          interest
      - in: query
        name: latitude
        description: Latitude of the center of the search, in decimal degrees
      - in: query
        name: longitude
        description: Longitude of the center of the search, in decimal degrees
      - in: query
        name: number_of_images
        description: Number of images to display
      - in: query
        name: number_of_results
        description: The maximum number of points of interest to return in the results
          set
      - in: query
        name: radius
        description: Radius around the center to look for points-of-interest around
          the given latitude and longitude in kilometers (km)
      - in: query
        name: social_media
        description: Enabling this includes images from Instagram in the output results
      - in: query
        name: vibes
        description: Includes content that doesnt correspond to an active physical
          place, but which gives the user some background information, or vibe for
          the place they are visiting
      responses:
        200:
          description: OK
      tags:
      - Points
      - Of
      - Interest
      - Yapq
      - Search
      - Circle
  /points-of-interest/yapq-search-text:
    get:
      summary: Get Points Of Interest Yapq Search Text
      description: "Amadeus has partnered with YapQ to bring you point of interest
        APIs with the goal of offering you unbiased ratings of landmarks and tourist
        attractions. YapQ rates these points according to their interest on social
        media and provides Wikipedia content and Geonames ID in a given city. \nYapQ's
        service indexes millions of points around the world, and provides content
        in 12 different languages. This allows you to ensure you catch the must-see
        sights in a YapQ supported city.\nEach point of interest comes with links
        to content, grading information, location and directions to help make discovering
        your destination easy and fun.\nThis service is still under active development,
        and the response format may change without warning. We'd be interested in
        your feedback - send us an email."
      operationId: getPointsOfInterestYapqSearchText
      x-api-path-slug: pointsofinterestyapqsearchtext-get
      parameters:
      - in: query
        name: category
        description: Filters the resulting points_of_interest to include only results
          which have a least one category containing the given provided word
      - in: query
        name: city_name
        description: The name of the supported city for which you are searching, in
          the selected language
      - in: query
        name: geonames
        description: Setting this to true includes only points of interest with a
          geonames ID
      - in: query
        name: image_size
        description: The size of the images youd like to see in the response
      - in: query
        name: lang
        description: The preferred language of the content related to each point of
          interest
      - in: query
        name: number_of_images
        description: Number of images to display
      - in: query
        name: number_of_results
        description: The maximum number of points of interest to return in the results
          set
      - in: query
        name: social_media
        description: Enabling this includes images from Instagram in the output results
      - in: query
        name: vibes
        description: Includes content that doesnt correspond to an active physical
          place, but which gives the user some background information, or vibe for
          the place they are visiting
      responses:
        200:
          description: OK
      tags:
      - Points
      - Of
      - Interest
      - Yapq
      - Search
      - Text
  /trains/extensive-search:
    get:
      summary: Get Trains Extensive Search
      description: "This API allows you to search trains availability and prices for
        a single day or date range. It's based on our Rail Instant Search technology,
        providing you with immediate results from our rail search cache.\n\nThis API
        has content from SNCF (French trains).\n            \nThe content is also
        restricted to single-leg trips - where a single train takes you directly from
        the origin to the destination."
      operationId: getTrainsExtensiveSearch
      x-api-path-slug: trainsextensivesearch-get
      parameters:
      - in: query
        name: departure_date
        description: The date or range of dates on which you would like to depart
          from the origin station to go to the destination
      - in: query
        name: destination
        description: Identifier of the rail station to which you would like to travel
      - in: query
        name: origin
        description: Identifier of the rail station from which you would like to depart
      responses:
        200:
          description: OK
      tags:
      - Trains
      - Extensive
      - Search
  /trains/schedule-search:
    get:
      summary: Get Trains Schedule Search
      description: |-
        This API allows you to find all the possible destinations in the Rail Instant Search cache (used by Extensive Search above) from a given origin station on a given day. You can use this to help build network maps, journey planners or provide inspiration for rail travel.

        This API has continuous content from SNCF.
        All the options returned are single-leg trips - where a single train takes you directly from the origin to the destination. In general, only departure dates up to 90 days in the future are supported

        Currently agglomeration stations are not supported
      operationId: getTrainsScheduleSearch
      x-api-path-slug: trainsschedulesearch-get
      parameters:
      - in: query
        name: departure_date
        description: The date on which you would like to depart from the origin station
          to go to the destination
      - in: query
        name: origin
        description: Identifier of the rail station where you would like to depart
          from
      responses:
        200:
          description: OK
      tags:
      - Trains
      - Schedule
      - Search