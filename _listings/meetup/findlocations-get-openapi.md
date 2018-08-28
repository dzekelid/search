---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Find locations
  description: Provides a query interface for finding known locations
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /find/events:
    get:
      summary: Find Events
      description: Returns list of upcoming events based on location
      operationId: deprecated
      x-api-path-slug: findevents-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to populate in the
          response
        type: string
      - in: query
        name: lat
        description: Approximate target latitude
        type: string
      - in: query
        name: lon
        description: Approximate target longitude
        type: string
      - in: query
        name: radius
        description: Radius in miles
        type: string
      - in: query
        name: text
        description: Raw full text search query
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
  /find/upcoming_events:
    get:
      summary: Find Upcoming Events
      description: Returns a list of upcoming events
      operationId: events
      x-api-path-slug: findupcoming-events-get
      parameters:
      - in: query
        name: end_date_range
        description: Return events that start before this date
        type: string
      - in: query
        name: end_time_range
        description: Return events that start before this time
        type: string
      - in: query
        name: excluded_groups
        description: IDs for groups to exclude from the returned events
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to populate in the
          response
        type: string
      - in: query
        name: lat
        description: Approximate target latitude
        type: string
      - in: query
        name: lon
        description: Approximate target longitude
        type: string
      - in: query
        name: order
        description: The sort order of returned events
        type: string
      - in: query
        name: page
        description: A target minimum number of events to return in a single page
          of results
        type: string
      - in: query
        name: radius
        description: Radius in miles
        type: string
      - in: query
        name: self_groups
        description: set to include or exclude or only get groups that the member
          belongs to
        type: string
      - in: query
        name: start_date_range
        description: Return events that start after this date
        type: string
      - in: query
        name: start_time_range
        description: Return events that start after this time
        type: string
      - in: query
        name: text
        description: Full text search query
        type: string
      - in: query
        name: topic_category
        description: Numeric topic category identifier for filtering recommendations
          by a topic category
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
  /find/groups:
    get:
      summary: Find Groups
      description: Text, location, category and friend-based group searches
      operationId: groups
      x-api-path-slug: findgroups-get
      parameters:
      - in: query
        name: category
        description: Comma-delimited list of numeric category ids
        type: string
      - in: query
        name: country
        description: A valid two character country code, defaults to US
        type: string
      - in: query
        name: fallback_suggestions
        description: boolean indicator of whether or not to return a list of curated
          suggestions for groups if we cant find groups matching your criteria
        type: string
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: filter
        description: Determines which groups are returned
        type: string
      - in: query
        name: lat
        description: Approximate latitude
        type: string
      - in: query
        name: location
        description: Raw text location query
        type: string
      - in: query
        name: lon
        description: Approximate longitude
        type: string
      - in: query
        name: radius
        description: Radius in miles
        type: string
      - in: query
        name: self_groups
        description: set to include or exclude Meetups the authorized member belongs
          to; default is include
        type: string
      - in: query
        name: text
        description: Raw full text search query
        type: string
      - in: query
        name: topic_id
        description: Comma-delimited list of numeric topic ids
        type: string
      - in: query
        name: upcoming_events
        description: If true, filters text and category based searches on groups that
          have upcoming events
        type: string
      - in: query
        name: zip
        description: Zipcode of location to limit search to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
      - Groups
  /find/venues:
    get:
      summary: Find Venues
      description: Returns list of venues based on location
      operationId: venues
      x-api-path-slug: findvenues-get
      parameters:
      - in: query
        name: country
        description: A valid two charater country code, desfaults to US
        type: string
      - in: query
        name: desc
        description: Boolean value to indicate to direction ordered results
        type: string
      - in: query
        name: fields
        description: Comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: lat
        description: Approximate latitude
        type: string
      - in: query
        name: location
        description: Raw text location query
        type: string
      - in: query
        name: lon
        description: Approximate longitude
        type: string
      - in: query
        name: radius
        description: Radius in miles
        type: string
      - in: query
        name: text
        description: Raw full text search query
        type: string
      - in: query
        name: zip
        description: Zipcode of location to limit search to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
      - Venues
  /find/:urlname/members:
    get:
      summary: Group Profile search
      description: |-
        Find group member profiles by name.
        Member's who very recently joined or left the group may not be immediately searchable
      operationId: profiles
      x-api-path-slug: findurlnamemembers-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: order
        description: Orders results according to definitions listed below
        type: string
      - in: query
        name: page
        description: Number of requested members to return
        type: string
      - in: query
        name: query
        description: The name to search for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Search
  /find/locations:
    get:
      summary: Find locations
      description: Provides a query interface for finding known locations
      operationId: geo
      x-api-path-slug: findlocations-get
      parameters:
      - in: query
        name: lat
        description: Search for locations based on location latitude
        type: string
      - in: query
        name: lon
        description: Search for locations based on location longitude
        type: string
      - in: query
        name: offset
        description: The current offset in the paginated set, represented as an incrementing
          value
        type: string
      - in: query
        name: page
        description: The desired number of locations to return in a single set of
          results
        type: string
      - in: query
        name: query
        description: Search for locations based on city name or zip code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
      - Location
x-streamrank:
  polling_total_time_average: "0.1"
  polling_size_download_average: "32232.91"
  streaming_total_time_average: "0.06"
  streaming_size_download_average: "16130.59"
  change_yes: "3"
  change_no: "2277"
  time_percentage: "42"
  size_percentage: "50"
  change_percentage: "0"
  last_run: "2018-05-12"
  days_run: "8"
  minute_run: "0"
---