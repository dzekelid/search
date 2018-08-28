---
swagger: "2.0"
x-collection-name: UK National Archives
x-complete: 0
info:
  title: Getty Images Search API Get Search Veos Creative
  description: Search for creative videos.
  version: "3.0"
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/search/events:
    get:
      summary: Get Search Events
      description: Search for events.
      operationId: getV3SearchEvents
      x-api-path-slug: v3searchevents-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: date_from
        description: Filters to events that start on or after this date
      - in: query
        name: date_to
        description: Filters to events that start on or before this date
      - in: query
        name: editorial_segment
        description: Filters to events with a matching editorial segment
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Filters to events related to this phrase
      responses:
        200:
          description: OK
      tags:
      - Search
      - Events
  /v3/search/images:
    get:
      summary: Get Search Images
      description: Search for both creative and editorial images.
      operationId: getV3SearchImages
      x-api-path-slug: v3searchimages-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: query
        name: age_of_people
        description: Filter based on the age of individuals in an image
      - in: query
        name: artists
        description: Search for images by specific artists (free-text, comma-separated
          list of artists)
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Provides searching based on specified collection(s)
      - in: query
        name: collection_codes
        description: Filter by collection codes (comma-separated list)
      - in: query
        name: color
        description: Filter based on predominant color in an image
      - in: query
        name: compositions
        description: Filter based on image composition
      - in: query
        name: embed_content_only
        description: Restrict search results to embeddable images
      - in: query
        name: ethnicity
        description: Filter search results based on the ethnicity of individuals in
          an image
      - in: query
        name: event_ids
        description: Filter based on specific events
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: file_types
        description: Return only images having a specific file type
      - in: query
        name: graphical_styles
        description: Filter based on graphical style of the image
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the image licensing model(s)
      - in: query
        name: minimum_size
        description: Filter based on minimum size requested
      - in: query
        name: number_of_people
        description: Filter based on the number of people in the image
      - in: query
        name: orientations
        description: Return only images with selected aspect ratios
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Search images using a search phrase
      - in: query
        name: prestige_content_only
        description: Restrict search results to prestige images
      - in: query
        name: product_types
        description: Filter images to those having product types from the selected
          list
      - in: query
        name: sort_order
        description: Select sort order of results
      - in: query
        name: specific_people
        description: Return only images associated with specific people (using a comma-delimited
          list)
      responses:
        200:
          description: OK
      tags:
      - Search
      - Images
  /v3/search/images/creative:
    get:
      summary: Get Search Images Creative
      description: Search for creative images only.
      operationId: getV3SearchImagesCreative
      x-api-path-slug: v3searchimagescreative-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: query
        name: age_of_people
        description: Filter based on the age of individuals in an image
      - in: query
        name: artists
        description: Search for images by specific artists (free-text, comma-separated
          list of artists)
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Use to include or exclude collections from search
      - in: query
        name: collection_codes
        description: Filter by collection codes (comma-separated list)
      - in: query
        name: color
        description: Filter based on predominant color in an image
      - in: query
        name: compositions
        description: Filter based on image composition
      - in: query
        name: embed_content_only
        description: Restrict search results to embeddable images
      - in: query
        name: ethnicity
        description: Filter search results based on the ethnicity of individuals in
          an image
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: file_types
        description: Return only images having a specific file type
      - in: query
        name: graphical_styles
        description: Filter based on graphical style of the image
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the image licensing model(s)
      - in: query
        name: minimum_size
        description: Filter based on minimum size requested
      - in: query
        name: number_of_people
        description: Filter based on the number of people in the image
      - in: query
        name: orientations
        description: Return only images with selected aspect ratios
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Search images using a search phrase
      - in: query
        name: prestige_content_only
        description: Restrict search results to prestige images
      - in: query
        name: product_types
        description: Filter images to those having product types from the selected
          list
      - in: query
        name: sort_order
        description: Select sort order of results
      responses:
        200:
          description: OK
      tags:
      - Search
      - Images
      - Creative
  /v3/search/images/editorial:
    get:
      summary: Get Search Images Editorial
      description: Search for editorial images only.
      operationId: getV3SearchImagesEditorial
      x-api-path-slug: v3searchimageseditorial-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: query
        name: age_of_people
        description: Filter based on the age of individuals in an image
      - in: query
        name: artists
        description: Search for images by specific artists (free-text, comma-separated
          list of artists)
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Use to include or exclude collections from search
      - in: query
        name: collection_codes
        description: Filter by collections (comma-separated list of collection codes)
      - in: query
        name: compositions
        description: Filter based on image composition
      - in: query
        name: date_from
        description: Return only images that are created on or after this date
      - in: query
        name: date_to
        description: Return only images that are created on or before this date
      - in: query
        name: editorial_segments
        description: Return only events with a matching editorial segment
      - in: query
        name: embed_content_only
        description: Restrict search results to embeddable images
      - in: query
        name: entity_uris
        description: specify linked data entity uri
      - in: query
        name: ethnicity
        description: Filter search results based on the ethnicity of individuals in
          an image
      - in: query
        name: event_ids
        description: Filter based on specific events
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: file_types
        description: Return only images having a specific file type
      - in: query
        name: graphical_styles
        description: Filter based on graphical style of the image
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: minimum_quality_rank
        description: Filter search results based on minimum quality ranking
      - in: query
        name: minimum_size
        description: Filter based on minimum size requested
      - in: query
        name: number_of_people
        description: Filter based on the number of people in the image
      - in: query
        name: orientations
        description: Return only images with selected aspect ratios
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Search images using a search phrase
      - in: query
        name: product_types
        description: Filter images to those having product types from the selected
          list
      - in: query
        name: sort_order
        description: Select sort order of results
      - in: query
        name: specific_people
        description: Return only images associated with specific people (using a comma-delimited
          list)
      responses:
        200:
          description: OK
      tags:
      - Search
      - Images
      - Editorial
  /v3/search/videos:
    get:
      summary: Get Search Veos
      description: Search for both creative and editorial videos.
      operationId: getV3SearchVeos
      x-api-path-slug: v3searchvideos-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: query
        name: age_of_people
        description: Provides filtering according to the age of individuals in a video
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Provides searching based on specified collection(s)
      - in: query
        name: collection_codes
        description: Provides filtering by collection code
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: format_available
        description: Filters according to the digital video format available on a
          film asset
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the video licensing model(s)
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: phrase
        description: Free-text search query
      - in: query
        name: product_types
        description: Provides filtering by a list of product types
      - in: query
        name: sort_order
        description: Allows sorting of results
      - in: query
        name: specific_people
        description: Provides filtering by specific peoples names
      responses:
        200:
          description: OK
      tags:
      - Search
      - Veos
  /v3/search/videos/creative:
    get:
      summary: Get Search Veos Creative
      description: Search for creative videos.
      operationId: getV3SearchVeosCreative
      x-api-path-slug: v3searchvideoscreative-get
      parameters:
      - in: header
        name: Accept-Language
        description: Specifies the language of result values
      - in: query
        name: age_of_people
        description: Provides filtering according to the age of individuals in a video
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Provides searching based on specified collection(s)
      - in: query
        name: collection_codes
        description: Provides filtering by collection code
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: format_available
        description: Filters according to the digital video format available on a
          film asset
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the video licensing model(s)
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: phrase
        description: Free-text search query
      - in: query
        name: product_types
        description: Allows filtering by a list of product types
      - in: query
        name: sort_order
        description: Allows sorting of results
      responses:
        200:
          description: OK
      tags:
      - Search
      - Veos
      - Creative
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