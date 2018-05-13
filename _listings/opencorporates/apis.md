---
name: OpenCorporates
description: OpenCorporates is a website which shares data on corporate entities as
  open data under the share-alike attribution Open Database License. It was created
  by Chris Taggart and Rob McKinnon, under the auspices of their company, Chrinon
  Ltd, and launched on 20 December 2010. It has the aims of creating a URL with such
  data for every corporate entity in the world, importing government data relating
  to companies and matching it to specific companies. The site also shows groups of
  companies which are legally part of the same conglomerate. Basic company information
  is available as open data in XML or JSON format.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/OpenCorporates.jpg
x-kinRank: "9"
x-alexaRank: ""
tags:
- Target
- Stack Network
- SMS
- My API Stack
- Finance
- Enterprise
- Corporate Data
- Business Intelligence
- Business
- Business
- API LIfeycle
created: "2018-05-13"
modified: "2018-05-13"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/opencorporates/apis.md
specificationVersion: "0.14"
apis:
- name: OpenCorporates Companies Search
  description: nThis returns a collection of companies whose name matches the given
    search term (submitted as :q in the query parameters)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/OpenCorporates.jpg
  humanURL: https://opencorporates.com/
  baseURL: http:://api.opencorporates.com/v0.4/
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/opencorporates/companies-search-get.md
x-common:
- type: x-base
  url: https://api.opencorporates.com/
- type: x-blog
  url: http://blog.opencorporates.com/
- type: x-blog-rss
  url: http://blog.opencorporates.com/feed/
- type: x-developer
  url: http://api.opencorporates.com/
- type: x-github
  url: https://github.com/openc
- type: x-pricing
  url: https://opencorporates.com/info/pricing
- type: x-status
  url: http://status.opencorporates.com/
- type: x-terms-of-service
  url: https://opencorporates.com/info/licence
- type: x-twitter
  url: https://twitter.com/opencorporates
- type: x-website
  url: https://opencorporates.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---