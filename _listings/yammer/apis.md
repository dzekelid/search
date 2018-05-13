---
name: Yammer
description: Discuss ideas, share updates, and crowdsource answers from coworkers
  around the globe. Yammer gives your team a faster, smarter way to connect and collaborate
  across your company.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/535_logo.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Microsoft
- Messaging
- Media
- Chat
- Bots
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/yammer/apis.yaml
specificationVersion: "0.14"
apis:
- name: Yammer API
  description: Discuss ideas, share updates, and crowdsource answers from coworkers
    around the globe
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/535_logo.png
  humanURL: ""
  baseURL: ://example.com//
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/yammer/yamuri-search-json-get.md
- name: Yammer API Search Request
  description: "The search resource will return a list of messages, users, topics
    and groups that match the user\u2019s search query.\n\n\n\nsearch - The search
    query.\n\npage - Only 20 results of each type will be returned for each page,
    but a total count is returned with each query. page=1 (the default) will return
    items 1-20, page=2 will return items 21-30, etc.\n\nnum_per_page - This allows
    you to limit the number of results of each type per page, up to a maximum of 20,
    the default value."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/535_logo.png
  humanURL: http://developer.yammer.com
  baseURL: http:://example.com//
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/yammer/yamuri-search-json-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/yammer/yamuri-search-json-get-postman.md
x-common:
- type: x-website
  url: http://developer.yammer.com
- type: x-blog
  url: http://blog.yammer.com
- type: x-blog-rss
  url: http://blog.yammer.com/blog/feed
- type: x-crunchbase
  url: http://www.crunchbase.com/company/yammer
- type: x-documentation
  url: https://developer.yammer.com/docs
- type: x-embeddable
  url: https://developer.yammer.com/docs/embed
- type: x-forum
  url: https://techcommunity.microsoft.com/t5/Yammer/ct-p/Yammer
- type: x-github
  url: https://github.com/yammer
- type: x-partners
  url: https://developer.yammer.com/v1.0/docs/yammer-partners
- type: x-status
  url: http://status.yammer.com/
- type: x-support
  url: https://developer.yammer.com/v1.0/page/support
- type: x-terms-of-service
  url: https://about.yammer.com/terms/
- type: x-twitter
  url: https://twitter.com/yammer
- type: x-website
  url: http://developer.yammer.com
- type: x-blog
  url: http://blog.yammer.com
- type: x-blog-rss
  url: http://blog.yammer.com/blog/feed
- type: x-crunchbase
  url: http://www.crunchbase.com/company/yammer
- type: x-documentation
  url: https://developer.yammer.com/docs
- type: x-embeddable
  url: https://developer.yammer.com/docs/embed
- type: x-forum
  url: https://techcommunity.microsoft.com/t5/Yammer/ct-p/Yammer
- type: x-github
  url: https://github.com/yammer
- type: x-partners
  url: https://developer.yammer.com/v1.0/docs/yammer-partners
- type: x-status
  url: http://status.yammer.com/
- type: x-support
  url: https://developer.yammer.com/v1.0/page/support
- type: x-terms-of-service
  url: https://about.yammer.com/terms/
- type: x-twitter
  url: https://twitter.com/yammer
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---