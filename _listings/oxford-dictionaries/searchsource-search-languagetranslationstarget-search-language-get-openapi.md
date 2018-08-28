---
swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 0
info:
  title: Oxford Dictionaries Retrieve possible translation matches to input
  description: Use this to find matches in our translation dictionaries.
  termsOfService: http://helloreverb.com/terms/
  version: 1.8.0
host: od-api-demo.oxforddictionaries.com:443
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/{source_lang}:
    get:
      summary: Retrieve possible matches to input
      description: Use this to retrieve possible [headword](documentation/glossary?term=headword)
        matches for a given string of text. The results are culculated using headword
        matching, fuzzy matching, and [lemmatization](documentation/glossary?term=lemma)
      operationId: getSearchSourceLang
      x-api-path-slug: searchsource-lang-get
      parameters:
      - in: query
        name: limit
        description: Limit the number of results per response
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Offset the start number of the result
      - in: query
        name: prefix
        description: Set prefix to true if youd like to get results only starting
          with search string
      - in: query
        name: q
        description: Search string
      - in: query
        name: regions
        description: If searching in English, filter words with specific region(s)
          either us or gb
      - in: path
        name: source_lang
        description: IANA language code
      responses:
        200:
          description: OK
      tags:
      - Search
      - Source
      - Lang
  /search/{source_search_language}/translations={target_search_language}:
    get:
      summary: Retrieve possible translation matches to input
      description: Use this to find matches in our translation dictionaries.
      operationId: getSearchSourceSearchLanguageTranslationsTargetSearchLanguage
      x-api-path-slug: searchsource-search-languagetranslationstarget-search-language-get
      parameters:
      - in: query
        name: limit
        description: Limit the number of results per response
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Offset the start number of the result
      - in: query
        name: prefix
        description: Set prefix to true if youd like to get results only starting
          with search string
      - in: query
        name: q
        description: Search string
      - in: query
        name: regions
        description: Filter words with specific region(s) E
      - in: path
        name: source_search_language
        description: IANA language code
      - in: path
        name: target_search_language
        description: IANA language code
      responses:
        200:
          description: OK
      tags:
      - Search
      - Source
      - Search
      - Language
      - Translations=target
      - Search
      - Language
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