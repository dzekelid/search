---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Search
  description: "Searches a site for any questions which fit the given criteria.\n
    \nThis method is intentionally quite limited. For more general searching, you
    should use a proper internet search engine restricted to the domain of the site
    in question.\n \nAt least one of tagged or intitle must be set on this method.
    nottagged is only used if tagged is also set, for performance reasons.\n \ntagged
    and nottagged are semi-colon delimited list of tags. At least 1 tag in tagged
    will be on each returned question if it is passed, making it the OR equivalent
    of the AND version of tagged on /questions.\n \nThe sorts accepted by this method
    operate on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n - relevance - matches the relevance
    tab on the site itself Does not accept min or max\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
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
      description: "Searches a site for any questions which fit the given criteria.\n
        \nThis method is intentionally quite limited. For more general searching,
        you should use a proper internet search engine restricted to the domain of
        the site in question.\n \nAt least one of tagged or intitle must be set on
        this method. nottagged is only used if tagged is also set, for performance
        reasons.\n \ntagged and nottagged are semi-colon delimited list of tags. At
        least 1 tag in tagged will be on each returned question if it is passed, making
        it the OR equivalent of the AND version of tagged on /questions.\n \nThe sorts
        accepted by this method operate on the follow fields of the question object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        - relevance - matches the relevance tab on the site itself Does not accept
        min or max\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: searches-a-site-for-any-questions-which-fit-the-given-criteria-this-method-is-intentionally-quite-li
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: intitle
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: nottagged
        description: String list (semicolon delimited)
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Search
x-streamrank:
  polling_total_time_average: "0.12"
  polling_size_download_average: "323.95"
  streaming_total_time_average: "0.07"
  streaming_size_download_average: "163.32"
  change_yes: "849"
  change_no: "969"
  time_percentage: "41"
  size_percentage: "50"
  change_percentage: "47"
  last_run: "2018-05-01"
  days_run: "1"
  minute_run: "0"
---