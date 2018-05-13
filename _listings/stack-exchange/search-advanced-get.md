---
swagger: "2.0"
info:
  title: Stack Exchange Advanced Search
  description: "Searches a site for any questions which fit the given criteria.\n
    \nSearch criteria are expressed using the following parameters:\n  - q - a free
    form text parameter, will match all question properties based on an undocumented
    algorithm.\n - accepted - true to return only questions with accepted answers,
    false to return only those without. Omit to elide constraint.\n - answers - the
    minimum number of answers returned questions must have.\n - body - text which
    must appear in returned questions' bodies.\n - closed - true to return only closed
    questions, false to return only open ones. Omit to elide constraint.\n - migrated
    - true to return only questions migrated away from a site, false to return only
    those not. Omit to elide constraint.\n - notice - true to return only questions
    with post notices, false to return only those without. Omit to elide constraint.\n
    - nottagged - a semicolon delimited list of tags, none of which will be present
    on returned questions.\n - tagged - a semicolon delimited list of tags, of which
    at least one will be present on all returned questions.\n - title - text which
    must appear in returned questions' titles.\n - user - the id of the user who must
    own the questions returned.\n - url - a url which must be contained in a post,
    may include a wildcard.\n - views - the minimum number of views returned questions
    must have.\n - wiki - true to return only community wiki questions, false to return
    only non-community wiki ones. Omit to elide constraint.\n  \nAt least one additional
    parameter must be set if nottagged is set, for performance reasons.\n \nThe sorts
    accepted by this method operate on the follow fields of the question object:\n
    - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
    - relevance - matches the relevance tab on the site itself Does not accept min
    or max\n  activity is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of questions."
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
  /search/advanced:
    get:
      summary: Advanced Search
      description: Searches a site for any questions which fit the given criteria
      operationId: searches-a-site-for-any-questions-which-fit-the-given-criteria-search-criteria-are-expressed-using-t
      parameters:
      - in: query
        name: accepted
      - in: query
        name: answers
      - in: query
        name: body
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: closed
      - in: query
        name: filter
        description: |-
          #Discussion

          The Stack Exchange API allows applications to exclude almost every field returned
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: |
          sort = activity => date
          sort = creation => date
          sort = votes => number
          sort = relevance => none
      - in: query
        name: migrated
      - in: query
        name: min
        description: |
          sort = activity => date
          sort = creation => date
          sort = votes => number
          sort = relevance => none
      - in: query
        name: notice
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
        name: q
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
        name: title
      - in: query
        name: todate
        description: Unix date
      - in: query
        name: url
      - in: query
        name: user
      - in: query
        name: views
      - in: query
        name: wiki
      responses:
        200:
          description: OK
      tags:
      - search
definitions:
  created_comment:
    properties:
      body:
        description: This is a default description.
        type: get
      body_markdown:
        description: This is a default description.
        type: get
      can_flag:
        description: This is a default description.
        type: get
      comment_id:
        description: This is a default description.
        type: get
      creation_date:
        description: This is a default description.
        type: get
      edited:
        description: This is a default description.
        type: get
      link:
        description: This is a default description.
        type: get
      owner:
        description: This is a default description.
        type: get
      post_id:
        description: This is a default description.
        type: get
      post_type:
        description: This is a default description.
        type: get
  error:
    properties:
      error_id:
        description: This is a default description.
        type: get
      error_message:
        description: This is a default description.
        type: get
      error_name:
        description: This is a default description.
        type: get
  info_object:
    properties:
      answers_per_minute:
        description: This is a default description.
        type: get
      api_revision:
        description: This is a default description.
        type: get
      badges_per_minute:
        description: This is a default description.
        type: get
      new_active_users:
        description: This is a default description.
        type: get
      questions_per_minute:
        description: This is a default description.
        type: get
      site:
        description: This is a default description.
        type: get
      total_accepted:
        description: This is a default description.
        type: get
      total_answers:
        description: This is a default description.
        type: get
      total_badges:
        description: This is a default description.
        type: get
      total_comments:
        description: This is a default description.
        type: get
  single_filter:
    properties:
      filter:
        description: This is a default description.
        type: get
      filter_type:
        description: This is a default description.
        type: get
      included_fields:
        description: This is a default description.
        type: get
  user:
    properties:
      about_me:
        description: This is a default description.
        type: get
      accept_rate:
        description: This is a default description.
        type: get
      account_id:
        description: This is a default description.
        type: get
      age:
        description: This is a default description.
        type: get
      answer_count:
        description: This is a default description.
        type: get
      badge_counts:
        description: This is a default description.
        type: get
      creation_date:
        description: This is a default description.
        type: get
      display_name:
        description: This is a default description.
        type: get
      down_vote_count:
        description: This is a default description.
        type: get
      is_employee:
        description: This is a default description.
        type: get
x-collection-name: Stack Exchange
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---