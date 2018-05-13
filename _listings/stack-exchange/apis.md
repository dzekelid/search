---
name: Stack Exchange
description: Stack Exchange is a network of question and answer websites on diverse
  topics in many different fields, each site covering a specific topic, where questions,
  answers, and users are subject to a reputation award process. The sites are modeled
  after Stack Overflow, a forum for computer programming questions that was the original
  site in this network. The reputation system is designed to allow the sites to be
  self-moderating.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/253_logo.png
x-kinRank: "8"
x-alexaRank: ""
tags:
- Streamrank
- Stack
- Question Answer
- Plug in
- My API Stack
- Media
- Imports
- Content
- Code
- Citations
- Answers
created: "2018-05-13"
modified: "2018-05-13"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange Advanced Search
  description: "Searches a site for any questions which fit the given criteria.\n
    \nSearch criteria are expressed using the following parameters:\n  - q - a free
    form text parameter, will match all question properties based on an undocumented
    algorithm.\n - accepted - true to return only questions with accepted answers,
    false to return only those without. Omit to elide constraint.\n - answers - the
    minimum number of answers returned questions must have.\n - body - text which
    must appear in returned questions' bodies.\n - closed - true to return only closed
    questions, false to return only open ones. Omit to elide constraint.\n - migrated
    - true to return only questions migrated away from a site, false to return only
    those not. Omit to elide constraint.\n - notice - true to return only questions
    with post notices, false to return only those without. Omit to elide constraint.\n
    - nottagged - a semicolon delimited list of tags, none of which will be present
    on returned questions.\n - tagged - a semicolon delimited list of tags, of which
    at least one will be present on all returned questions.\n - title - text which
    must appear in returned questions' titles.\n - user - the id of the user who must
    own the questions returned.\n - url - a url which must be contained in a post,
    may include a wildcard.\n - views - the minimum number of views returned questions
    must have.\n - wiki - true to return only community wiki questions, false to return
    only non-community wiki ones. Omit to elide constraint.\n  \nAt least one additional
    parameter must be set if nottagged is set, for performance reasons.\n \nThe sorts
    accepted by this method operate on the follow fields of the question object:\n
    - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
    - relevance - matches the relevance tab on the site itself Does not accept min
    or max\n  activity is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/253_logo.png
  humanURL: https://stackexchange.com/
  baseURL: https://api.stackexchange.com//2.2
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/stack-exchange/search-advanced-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/stack-exchange/search-advanced-get-postman.md
x-common:
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---