---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 0
info:
  title: Getty Images Search Editorial Videos
  description: "Use this endpoint to search over a blend of our premium stock, contemporary
    4K and HD footage, celebrities, news, newsmakers, entertainment, events and archival
    videos.\r\n\r\nYou'll need an API key and access token to use this resource. Please
    see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n\r\nYou can
    show different information in the response by specifying values on the \"fields\"
    parameter (see details below).\r\nYou can search with only an API key, and that
    will give you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to build search response results. The following
    fields are provided for every video in your result set when you include **summary_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a detailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n
    \   [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",\r\n
    \       \"caption\",\r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\",\r\n        \"color_type\",\r\n
    \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"era\",\r\n
    \       \"license_model\",\r\n        \"mastered_to\",\r\n        \"originally_shot_on\",\r\n
    \       \"product_types\",\r\n        \"shot_speed\",\r\n        \"source\",\r\n
    \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution files that are most frequently used
    to build a UI displaying search results. The following fields are provided for
    every video in your result set when you include **display_set** in your request.\r\n\r\n```\r\n{\r\n
    \   \"videos\":\r\n    [\r\n        \"display_sizes\":\r\n        [\r\n            {\r\n
    \               \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\":
    \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n
    \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
    Specifying the \"entity_details\" response field can have significant performance
    implications. The field should be used only when necessary."
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
  /v3/search/images/creative:
    get:
      summary: Search for creative images only
      description: "Use this endpoint to search our contemporary stock photos, illustrations
        and archival images.\r\n\r\nYou'll need an API key and access token to use
        this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        \r\npage for more information on how to sign up for an API key. \r\n \r\nYou
        can show different information in the response by specifying values on the
        \"fields\" parameter (see details below).\r\nYou can search with only an API
        key, and that will give you search results that are equivalent to doing a
        search on the GettyImages.com site without being logged in (anonymous search).
        \ If you are a Getty Images API customer and would like to ensure that your
        API searches return only assets that you have a license to use, you need to
        also include an authorization token in the header of your request.  Please
        consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
        sets are used in the **fields** request parameter to receive a suite of metadata
        fields. The following fields sets are available:\r\n\r\n#### Summary Fields
        Set\r\n\r\nThe **summary_set** query string parameter fields value represents
        a small batch of metadata fields that are often used to \r\nbuild search response
        results. The following fields are provided for every image in your result
        set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\": \r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"thumb\"\r\n            }\r\n        ],\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to \r\nbuild
        a detailed view of images. The following fields are provided for every image
        in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\": \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":
        \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n
        \       \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"orientation\",\r\n        \"product_types\",\r\n        \"quality_rank\",\r\n
        \       \"referral_destinations\",\r\n        \"title\"\r\n    ]\r\n]\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution\r\nfiles
        that are most frequently used to build a UI displaying search results. The
        following fields are provided for every image \r\nin your result set when
        you include **display_set** in your request.\r\n\r\n```Go\r\n{\r\n    \"images\":
        \r\n    [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n
        \               \"name\": \"comp\"\r\n            },\r\n            {\r\n
        \               \"name\": \"preview\"\r\n            },\r\n            {\r\n
        \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```"
      operationId: Search_GetCreativeImagesByPhrase
      x-api-path-slug: v3searchimagescreative-get
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
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Select sort order of results
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
  /v3/search/images/creative/by-image:
    get:
      summary: Search Images by Image
      description: "Allows searching for similar creative images by passing the URL
        to an existing image.\r\n\r\nBefore calling the search by image endpoint,
        an image must be uploaded to a specific AWS S3 bucket. The bucket name is
        `search-by-image.s3.amazonaws.com`.\r\nFor example, using cURL:\r\n```sh\r\ncurl
        -i -X PUT https://search-by-image.s3.amazonaws.com/my-test-image.jpg -H \"Content-Type:
        image/jpeg\" --data-binary \"@testimage.jpg\"\r\n```\r\n\r\nUploads can be
        overwritten if the names are the same, so using a prefix like the API Key,
        application name or company name would help keep that\r\nfrom happening.\r\n\r\nOnce
        the image has been uploaded, use the full URL in the `image_url` parameter,
        e.g. `image_url=https://search-by-image.s3.amazonaws.com/my-test-image.jpg`.\r\n\r\nSubsequent
        searches for the same image can be executed using the `image_fingerprint`
        that is returned by the inital search."
      operationId: Search_GetCreativeImagesByUrl
      x-api-path-slug: v3searchimagescreativebyimage-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: image_fingerprint
        description: Specifies the fingerprint of the image to use in the search
      - in: query
        name: image_url
        description: Specifies the location of the image to use in the search
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
  /v3/search/images/editorial:
    get:
      summary: Search Editorial Images
      description: Use this endpoint to search our editorial stock photos, illustrations
        and archival images.  Editorial images represent newsworthy events or illustrate
        matters of general interest, such as news, sport and entertainment and are
        generally intended for editorial use.
      operationId: Search_GetEditorialImagesByPhrase
      x-api-path-slug: v3searchimageseditorial-get
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
        description: Use to include or exclude collections from search
      - in: query
        name: collection_codes
        description: Filter by collections (comma-separated list of collection codes)
      - in: query
        name: compositions
        description: Filter based on image composition
      - in: query
        name: editorial_segments
        description: Return only events with a matching editorial segment
      - in: query
        name: embed_content_only
        description: Restrict search results to embeddable images
      - in: query
        name: end_date
        description: Return only images that are created on or before this date
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
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Select sort order of results
      - in: query
        name: specific_people
        description: Return only images associated with specific people (using a comma-delimited
          list)
      - in: query
        name: start_date
        description: Return only images that are created on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
      - Editorial
  /v3/search/videos:
    get:
      summary: Search Editorial Videos
      description: "Use this endpoint to search over a blend of our premium stock,
        contemporary 4K and HD footage, celebrities, news, newsmakers, entertainment,
        events and archival videos.\r\n\r\nYou'll need an API key and access token
        to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\n\r\nYou
        can show different information in the response by specifying values on the
        \"fields\" parameter (see details below).\r\nYou can search with only an API
        key, and that will give you search results that are equivalent to doing a
        search on the GettyImages.com site without being logged in (anonymous search).
        \ If you are a Getty Images API customer and would like to ensure that your
        API searches return only assets that you have a license to use, you need to
        also include an authorization token in the header of your request.  Please
        consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
        sets are used in the **fields** request parameter to receive a suite of metadata
        fields. The following fields sets are available:\r\n\r\n#### Summary Fields
        Set\r\n\r\nThe **summary_set** query string parameter fields value represents
        a small batch of metadata fields that are often used to build search response
        results. The following fields are provided for every video in your result
        set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\":\r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_name\",\r\n        \"display_sizes\":\r\n
        \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a detailed view of videos. The following fields are provided for every video
        in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\":\r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"caption\",\r\n        \"clip_length\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"color_type\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
        \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ],\r\n        \"era\",\r\n        \"license_model\",\r\n
        \       \"mastered_to\",\r\n        \"originally_shot_on\",\r\n        \"product_types\",\r\n
        \       \"shot_speed\",\r\n        \"source\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution
        files that are most frequently used to build a UI displaying search results.
        The following fields are provided for every video in your result set when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n
        \   [\r\n        \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Search_GetVideosByPhrase
      x-api-path-slug: v3searchvideos-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
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
        name: editorial_video_types
        description: Allows filtering by types of video
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
        name: frame_rates
        description: Provides filtering by video frame rate (frames/second)
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
        description: Filter images to those from one of your product types
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
      - Images
      - Search
      - Videos
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