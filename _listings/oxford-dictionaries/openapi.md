swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 1
info:
  title: Oxford Dictionaries
  description: if-youre-looking-to-enhance-your-app-or-website-with-dictionary-data-dont-compromise-on-quality--the-oxford-dictionaries-api-offers-easy-and-intuitive-access-to-oxfords-dictionary-content-which-is-trusted-around-the-world--here-at-oxford-dictionaries-home-of-the-oed-we-love-words--thats-why-we-have-experienced-lexicographers-tracking-the-living-language-delving-deep-into-our-corpora-and-monitoring-a-wide-range-of-media-in-order-to-understand-how-words-are-being-used-and-how-language-is-evolving--this-research-is-used-by-our-editors-to-write-and-edit-dictionary-entries-and-translations-meaning-were-able-to-offer-uptodate-accurate-and-reliable-lexical-content-in-multiple-languages-
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
  /search/{source_lang}/translations={target_lang}:
    get:
      summary: Find translation results for search query.
      description: Find available translation results  for a search query and language.
      operationId: getSearchSourceLangTranslationsTargetLang
      x-api-path-slug: searchsource-langtranslationstarget-lang-get
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
      responses:
        200:
          description: OK
      tags:
      - Search
      - Source
      - Lang
      - Translations=target
      - Lang