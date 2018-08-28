---
name: BC Laws
x-slug: bc-laws
description: 'BC Laws is an electronic library providing free public access to the
  laws of British Columbia. BC Laws is hosted by the Queen&rsquo;s Printer of British
  Columbia and published in partnership with the Ministry of Justice and the Law Clerk
  of the Legislative Assembly. BC Laws contains a comprehensive collection of BC legislation
  and related materials. It is available on the internet in two forms: First: The
  library is available as a web site in which users can browse and search the laws
  of British Columbia. Second: The library is available as a portal to legislation
  in raw XML1 data format, accessible via the BC Laws API2. This direct access to
  raw data is intended to enable third parties to build or add their own custom applications
  based on the structure of the data and all the associated search functionality inherent
  in that structure. The BC Laws website itself is an example of one such application.'
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Search
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/bc-laws/apis.md
specificationVersion: "0.14"
apis:
- name: BC Laws - Retrieves a specific document from the BCLaws legislative repository
    with search text highlighted (HTML format)
  x-api-slug: documentidaspectidcivixindexidcivixdocumentidsearchsearchstring-get
  description: 'The /document API allows you to retrieve actual documents from the
    BCLaws legislative repository. To retrieve a document from the repository you
    need the aspect identifier and two other specific pieces of information about
    the document: the index identifier and the document identifier. These unique identifiers
    can be retrieved from the /content API.'
  image: ""
  humanURL: http://bclaws.ca
  baseURL: https://www.bclaws.ca//civix
  tags: Laws, State Government, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/bc-laws/documentidaspectidcivixindexidcivixdocumentidsearchsearchstring-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/bc-laws/documentidaspectidcivixindexidcivixdocumentidsearchsearchstring-get-openapi.md
- name: BC Laws - Retrieves a specific document from the BCLaws legislative repository
    with search text highlighted (XML format)
  x-api-slug: documentidaspectidcivixindexidcivixdocumentidxmlsearchsearchstring-get
  description: 'The /document API allows you to retrieve actual documents from the
    BCLaws legislative repository. To retrieve a document from the repository you
    need the aspect identifier and two other specific pieces of information about
    the document: the index identifier and the document identifier. These unique identifiers
    can be retrieved from the /content API.'
  image: ""
  humanURL: http://bclaws.ca
  baseURL: https://www.bclaws.ca//civix
  tags: Laws, State Government, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/bc-laws/documentidaspectidcivixindexidcivixdocumentidxmlsearchsearchstring-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/bc-laws/documentidaspectidcivixindexidcivixdocumentidxmlsearchsearchstring-get-openapi.md
- name: BC Laws - A listing of metadata available for the specified aspect and search
    term from the BCLaws legislative repository
  x-api-slug: searchaspectidfullsearch-get
  description: A listing of metadata available for the specified aspect and search
    term from the BCLaws legislative repository
  image: ""
  humanURL: http://bclaws.ca
  baseURL: https://www.bclaws.ca//civix
  tags: Laws, State Government, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/bc-laws/searchaspectidfullsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/bc-laws/searchaspectidfullsearch-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bc.geographical.names.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bc.laws.stack.network
- type: x-website
  url: http://bclaws.ca
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---