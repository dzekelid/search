---
name: Getty Images
x-slug: getty-images
description: Find high resolution royalty-free images, editorial stock photos, vector
  art, video footage clips and stock music licensing at the richest image search photo
  library online.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
x-kinRank: "8"
x-alexaRank: "1939"
tags: Search
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images - Search for events
  x-api-slug: v3searchevents-get
  description: "Use this endpoint to search Getty Images news, sports and entertainment
    events. Getty Images photographers and videographers cover editorially relevant
    events occurring around the world.  All images or video clips produced in association
    with an event, are assigned the same EventID. EventIDs are part of the meta-data
    returned in Search Results. Only content produced under a Getty Images brand name
    (Getty Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
    Wire Image) will be consistently assigned an EventID. The Event framework may
    also be used to group similar content, such as \"Hats from the Royal Wedding\"
    or \"Odd-ballOffbeat images of the week\".   \r\n\r\nYou'll need an API key and
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n\r\nYou can
    show different information in the response by specifying values on the \"fields\"
    parameter (see details below).\r\nYou can search with only an API key, and that
    will give you search results that are equivalent to doing a search on the GettyImages.com
    site without being logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only assets that
    you have a license to use, you need to also include an authorization token in
    the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
    for code examples of getting a token."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchevents-get-openapi.md
- name: Getty Images - Search Images
  x-api-slug: v3searchimages-get
  description: Use this endpoint to search over a blend of our contemporary stock
    photos, illustrations, archival images, editorial photos, illustrations and archival
    images.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimages-get-openapi.md
- name: Getty Images - Search for creative images only
  x-api-slug: v3searchimagescreative-get
  description: "Use this endpoint to search our contemporary stock photos, illustrations
    and archival images.\r\n\r\nYou'll need an API key and access token to use this
    resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    \r\npage for more information on how to sign up for an API key. \r\n \r\nYou can
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
    metadata fields that are often used to \r\nbuild search response results. The
    following fields are provided for every image in your result set when you include
    **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\": \r\n    [\r\n
    \       \"asset_family\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\",\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n
    \   ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query
    string parameter fields value represents a large batch of metadata fields that
    are often used to \r\nbuild a detailed view of images. The following fields are
    provided for every image in your result set when you include **detail_set** in
    your request.\r\n\r\n```\r\n{\r\n    \"images\": \r\n    [\r\n        \"allowed_use\",\r\n
    \       \"artist\",\r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n
    \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n
    \       \"collection_name\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
    \       \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n        \"graphical_style\",\r\n
    \       \"license_model\",\r\n        \"max_dimensions\",\r\n        \"orientation\",\r\n
    \       \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n
    \       \"title\"\r\n    ]\r\n]\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution\r\nfiles that are most frequently
    used to build a UI displaying search results. The following fields are provided
    for every image \r\nin your result set when you include **display_set** in your
    request.\r\n\r\n```Go\r\n{\r\n    \"images\": \r\n    [\r\n        \"display_sizes\":
    \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimagescreative-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimagescreative-get-openapi.md
- name: Getty Images - Search Images by Image
  x-api-slug: v3searchimagescreativebyimage-get
  description: "Allows searching for similar creative images by passing the URL to
    an existing image.\r\n\r\nBefore calling the search by image endpoint, an image
    must be uploaded to a specific AWS S3 bucket. The bucket name is `search-by-image.s3.amazonaws.com`.\r\nFor
    example, using cURL:\r\n```sh\r\ncurl -i -X PUT https://search-by-image.s3.amazonaws.com/my-test-image.jpg
    -H \"Content-Type: image/jpeg\" --data-binary \"@testimage.jpg\"\r\n```\r\n\r\nUploads
    can be overwritten if the names are the same, so using a prefix like the API Key,
    application name or company name would help keep that\r\nfrom happening.\r\n\r\nOnce
    the image has been uploaded, use the full URL in the `image_url` parameter, e.g.
    `image_url=https://search-by-image.s3.amazonaws.com/my-test-image.jpg`.\r\n\r\nSubsequent
    searches for the same image can be executed using the `image_fingerprint` that
    is returned by the inital search."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimagescreativebyimage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimagescreativebyimage-get-openapi.md
- name: Getty Images - Search Editorial Images
  x-api-slug: v3searchimageseditorial-get
  description: Use this endpoint to search our editorial stock photos, illustrations
    and archival images.  Editorial images represent newsworthy events or illustrate
    matters of general interest, such as news, sport and entertainment and are generally
    intended for editorial use.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimageseditorial-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchimageseditorial-get-openapi.md
- name: Getty Images - Search Editorial Videos
  x-api-slug: v3searchvideos-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchvideos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchvideos-get-openapi.md
- name: Getty Images - Search for creative videos
  x-api-slug: v3searchvideoscreative-get
  description: "Use this endpoint to search premium stock video, from archival film
    to contemporary 4K and HD footage.\r\n\r\nYou'll need an API key and access token
    to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
    for more information on how to sign up for an API key.\r\n\r\nYou can show different
    information in the response by specifying values on the \"fields\" parameter (see
    details below).\r\nYou can search with only an API key, and that will give you
    search results that are equivalent to doing a search on the GettyImages.com site
    without\r\nbeing logged in (anonymous search).  If you are a Getty Images API
    customer and would like to ensure that your API searches return only \r\nassets
    that you have a license to use, you need to also include an authorization token
    in the header of your request.\r\nPlease consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
    for more information on authorization tokens.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
    sets are used in the **fields** request parameter to receive a suite of metadata
    fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe
    **summary_set** query string parameter fields value represents a small batch of
    metadata fields that are often used to build search\r\nresponse results. The following
    fields are provided for every video in your result set when you include **summary_set**
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\": \r\n    [\r\n        \"asset_family\",
    \r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a \r\ndetailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":
    \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",
    \r\n        \"caption\", \r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\", \r\n        \"color_type\",\r\n
    \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"era\",\r\n
    \       \"license_model\",\r\n        \"mastered_to\",\r\n        \"originally_shot_on\",\r\n
    \       \"product_types\",\r\n        \"shot_speed\",\r\n        \"source\",\r\n
    \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
    **display_set** query string parameter fields value represents the fields that
    provide you with URLs for the low resolution files \r\nthat are most frequently
    used to build a UI displaying search results. The following fields are provided
    for every video in your result \r\nset when you include **display_set** in your
    request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"display_sizes\":\r\n
    \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
    \           {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n
    \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchvideoscreative-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchvideoscreative-get-openapi.md
- name: Getty Images - Search for editorial videos
  x-api-slug: v3searchvideoseditorial-get
  description: "Use this endpoint to search current and archival video clips of celebrities,
    newsmakers, and events.\r\n\r\nYou'll need an API key and access token to use
    this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\nYou can show
    different information in the response by specifying values on the \"fields\" parameter
    (see details below).\r\nYou can search with only an API key, and that will give
    you search results that are equivalent to doing a search on the GettyImages.com
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
    in your request.\r\n\r\n```\r\n{\r\n    \"videos\": \r\n    [\r\n        \"asset_family\",
    \r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_name\",\r\n
    \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
    \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
    \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n
    \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
    Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value
    represents a large batch of metadata fields that are often used to build a detailed
    view of videos. The following fields are provided for every video in your result
    set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":
    \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",
    \r\n        \"caption\", \r\n        \"clip_length\",\r\n        \"collection_code\",\r\n
    \       \"collection_id\",\r\n        \"collection_name\", \r\n        \"color_type\",\r\n
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Images, Stack Network, Videos, Photos, Getting Started Example, Media, internet,
    Technology, Marketplace, API Provider, Stocks, Photos, Photos, Photos, Profiles,
    Publish, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchvideoseditorial-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/getty-images/v3searchvideoseditorial-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://getstream.io.api.gallery.streamdata.io
- type: x-api-stack
  url: http://getty.images.stack.network
- type: x-authentication
  url: https://github.com/gettyimages/connect#authentication
- type: x-base
  url: https://connect.gettyimages.com/
- type: x--net-sdk
  url: https://github.com/gettyimages/connect_sdk_csharp
- type: x-crunchbase
  url: https://crunchbase.com/organization/gettyimages
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ge-tt
- type: x-developer
  url: http://api.gettyimages.com/
- type: x-documentation
  url: https://api.gettyimages.com/swagger/ui/index.html
- type: x-email
  url: privacy@gettyimages.com
- type: x-email
  url: sales@gettyimages.com
- type: x-email
  url: copyright@gettyimages.com
- type: x-embeddable
  url: https://github.com/gettyimages/connect#oembed
- type: x-forum
  url: http://api.gettyimages.com/forum
- type: x-getting-started
  url: https://github.com/gettyimages/connect#getting-started
- type: x-github
  url: https://github.com/gettyimages
- type: x-java-sdk
  url: https://github.com/gettyimages/connect_sdk_java
- type: x-node-js-sdk
  url: https://github.com/gettyimages/connect_sdk_nodejs
- type: x-objectivec-sdk
  url: https://github.com/gettyimages/connect_sdk_objective-c
- type: x-php-sdk
  url: https://github.com/gettyimages/connect_sdk_php
- type: x-pricing
  url: http://www.gettyimages.com/subscribe
- type: x-ruby-sdk
  url: https://github.com/gettyimages/connect_sdk_ruby
- type: x-twitter
  url: https://twitter.com/GettyImages
- type: x-website
  url: http://www.gettyimages.com/
- type: x-website
  url: http://gettyimages.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---