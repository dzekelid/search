---
name: Flickr
x-slug: flickr
description: Flickr (pronounced flicker) is an image hosting and video hosting website,
  and web services suite that was created by Ludicorp in 2004 and acquired by Yahoo
  in 2005. In addition to being a popular website for users to share and embed personal
  photographs, and effectively an online community, the service is widely used by
  photo researchers and by bloggers to host images that they embed in blogs and social
  media.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Search
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/flickr/apis.md
specificationVersion: "0.14"
apis:
- name: Flickr - Groups Search
  x-api-slug: restmethodflickr-groups-search-get
  description: Search for groups. 18+ groups will only be returned for authenticated
    calls where the authenticated user is over 18.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services/
  tags: Images, My API Stack, Imports, Stack Network, Stack, Media, Photos, Getting
    Started Example, API Provider, Photos, Photos, Profiles, General Data, Relative
    Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/flickr/restmethodflickr-groups-search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/flickr/restmethodflickr-groups-search-get-openapi.md
- name: Flickr - Photos Search
  x-api-slug: restmethodflickr-photos-search-get
  description: Return a list of photos matching some criteria. Only photos visible
    to the calling user will be returned. To return private or semi-private photos,
    the caller must be authenticated with 'read' permissions, and have permission
    to view the photos. Unauthenticated calls will only return public photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services/
  tags: Images, My API Stack, Imports, Stack Network, Stack, Media, Photos, Getting
    Started Example, API Provider, Photos, Photos, Profiles, General Data, Relative
    Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/flickr/restmethodflickr-photos-search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/flickr/restmethodflickr-photos-search-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://flat.api.gallery.streamdata.io
- type: x-api-stack
  url: http://flickr.stack.network
- type: x-authentication
  url: https://www.flickr.com/services/api/auth.oauth.html
- type: x-base
  url: https://api.flickr.com/services/
- type: x-developer
  url: https://www.flickr.com/services/api/
- type: x-getting-started
  url: https://www.flickr.com/services/developer/
- type: x-privacy
  url: https://info.yahoo.com/privacy/us/yahoo/flickr/details.html
- type: x-support
  url: https://help.yahoo.com/kb/flickr-for-desktop
- type: x-terms-of-service
  url: https://www.flickr.com/services/api/tos/
- type: x-twitter
  url: https://twitter.com/flickr
- type: x-website
  url: http://www.flickr.com/
- type: x-website
  url: http://flickr.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---