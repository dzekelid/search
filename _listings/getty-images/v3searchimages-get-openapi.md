---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 0
info:
  title: Getty Images Search Images
  description: Use this endpoint to search over a blend of our contemporary stock
    photos, illustrations, archival images, editorial photos, illustrations and archival
    images.
  version: 1.0.0
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
      summary: Search for events
      description: "Use this endpoint to search Getty Images news, sports and entertainment
        events. Getty Images photographers and videographers cover editorially relevant
        events occurring around the world.  All images or video clips produced in
        association with an event, are assigned the same EventID. EventIDs are part
        of the meta-data returned in Search Results. Only content produced under a
        Getty Images brand name (Getty Images News, Getty Images Sports, Getty Images
        Entertainment, Film Magic, Wire Image) will be consistently assigned an EventID.
        The Event framework may also be used to group similar content, such as \"Hats
        from the Royal Wedding\" or \"Odd-ballOffbeat images of the week\".   \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key.\r\n\r\n\r\nYou can show
        different information in the response by specifying values on the \"fields\"
        parameter (see details below).\r\nYou can search with only an API key, and
        that will give you search results that are equivalent to doing a search on
        the GettyImages.com site without being logged in (anonymous search).  If you
        are a Getty Images API customer and would like to ensure that your API searches
        return only assets that you have a license to use, you need to also include
        an authorization token in the header of your request.  Please consult our
        [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token."
      operationId: Search_GetEvents
      x-api-path-slug: v3searchevents-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
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
        description: Request results starting at a page number (default is 1, maximum
          is 50)
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
      - Images
      - Search
  /v3/search/images:
    get:
      summary: Search Images
      description: Use this endpoint to search over a blend of our contemporary stock
        photos, illustrations, archival images, editorial photos, illustrations and
        archival images.
      operationId: Search_GetImagesByPhrase
      x-api-path-slug: v3searchimages-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
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
        description: Filter images to those from one of your product types
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
      - Images
      - Search
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