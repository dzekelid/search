---
swagger: "2.0"
x-collection-name: Wordnik
x-complete: 0
info:
  title: Wordnik Searches words
  description: Searches words.
  version: "4.0"
host: api.wordnik.com
basePath: /v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /words.json/search/{query}:
    get:
      summary: Searches words
      description: Searches words.
      operationId: searchWords
      x-api-path-slug: words-jsonsearchquery-get
      parameters:
      - in: query
        name: caseSensitive
        description: Search case sensitive
      - in: query
        name: excludePartOfSpeech
        description: Exclude these comma-delimited parts of speech
      - in: query
        name: includePartOfSpeech
        description: Only include these comma-delimited parts of speech
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: maxCorpusCount
        description: Maximum corpus frequency for terms
      - in: query
        name: maxDictionaryCount
        description: Maximum dictionary definition count
      - in: query
        name: maxLength
        description: Maximum word length
      - in: query
        name: minCorpusCount
        description: Minimum corpus frequency for terms
      - in: query
        name: minDictionaryCount
        description: Minimum number of dictionary entries for words returned
      - in: query
        name: minLength
        description: Minimum word length
      - in: path
        name: query
        description: Search query
      - in: query
        name: skip
        description: Results to skip
      responses:
        200:
          description: OK
      tags:
      - Words
      - Search
      - Query
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