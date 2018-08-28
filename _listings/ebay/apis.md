---
name: eBay
x-slug: ebay
description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
  goods, digital cameras, baby items, coupons, and everything else on eBay, the worlds
  online marketplace
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
x-kinRank: "8"
x-alexaRank: "42"
tags: Search
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/ebay/apis.md
specificationVersion: "0.14"
apis:
- name: Ebay - Get Item Summary Search
  x-api-slug: item-summarysearch-get
  description: 'This call performs an advanced search for items. You can search by
    keyword, category, eBay product Id (EPID), or gtin. Or a combination of these.
    Encoding Parameters and Headers As with all query parameter values, the fields
    parameter value and request header values must be URL encoded. For better readability,
    the examples in this document omit the encoding. Example: &nbsp;&nbsp;search?q=world
    cup soccer ball&amp;aspect_filter=categoryId:20863,Brand:{Nike|Wilson} Encoded
    Example: &nbsp;&nbsp; search?q=world cup soccer ball&amp;aspect_filter=categoryId%3A20863%2CBrand%3A%7BNike%7CWilson%7D
    For more information about encoding, see HTML URL Encoding Reference The following
    are examples of using filters: The following call returns 4,330,774 items. &nbsp;&nbsp;&nbsp;/buy/browse/v1/item_summary/search?q=phone
    This call, which limits the results to the category &quot;Cell Phones &amp; Smartphones&quot;,
    returns 142,098 items. &nbsp;&nbsp;&nbsp;/buy/browse/v1/item_summary/search?q=phone&amp;category_ids=9355
    These calls, which limit results to a Samsung Galaxy S5, returns 97 items. &nbsp;&nbsp;&nbsp;/buy/browse/v1/item_summary/search?q=phone&amp;category_ids=220&amp;epid=182527490
    &nbsp;&nbsp;&nbsp;or &nbsp;&nbsp;&nbsp;/buy/browse/v1/item_summary/search?epid=182527490
    Controlling what is returned You can also control what is returned by using the
    fieldgroups field. In addition to returning items, which is the default, you can
    return refinements (metadata) about an item that enables you to create aspect
    histograms. A histogram enables users to drill down in each refinement narrowing
    the search results. You can return: ASPECT_REFINEMENTS - Lets shoppers refine
    the result set by variation aspects, such as Brand, Color, etc. BUYING_OPTION_REFINEMENT
    - Lets shoppers refine the result set by either FIXED_PRICE or AUCTION CATEGORY_REFINEMENTS
    - Lets shoppers refine the result set by items in a category CONDITION_REFINEMENT
    - Lets shoppers refine the result set by item condition, such as NEW, USED, etc.
    MATCHING_ITEMS - The default, which returns the items. When used with one or more
    of the refinement values above the specified refinements and all the matching
    items are returned. FULL - This returns all the refinement containers and all
    the matching items. Filtering by aspects You can use the aspect refinements returned
    to filter the result set using the aspect_filter field. For example: This call
    gets a list of the aspects pairs for the item and the dominant category (category
    most of the items are in). /buy/browse/v1/item_summary/search?q=world cup soccer
    ball&amp;fieldgroups=ASPECT_REFINEMENTS This call filters the items by one of
    the aspect pairs returned and the dominant category ( categoryId is required when
    using aspect_filter) /buy/browse/v1/item_summary/search?q=world cup soccer ball&amp;aspect_filter=categoryId:20863,Brand:{adidas}
    This call filters the items by multiple aspects /buy/browse/v1/item_summary/search?q=world
    cup soccer ball&amp;aspect_filter=categoryId:20863,Brand:{adidas},Featured Refinements:{Adidas
    Match Ball} This call filters the items by multiple aspect values /buy/browse/v1/item_summary/search?q=world
    cup soccer ball&amp;aspect_filter=categoryId:20863,Brand:{Nike|Wilson} Additional
    filters There are also multiple filters you can use to refine the result set,
    such as listing format, item condition, price range, listing end date, location,
    and more. You can use multiple filters in a single call. For a list and details
    of the supported filters, see search Call Field Filters. Pagination and sort controls
    There are pagination controls ( limit and offset fields) and sort query parameter
    that control/sort the data that is returned. By default, the results are sorted
    by &quot;Best Match&quot;. For more information about Best Match, see the eBay
    help page Best Match. Request headers You will want to use the X-EBAY-C-ENDUSERCTX
    request header with this call. If you are an eBay Network Partner you must use
    affiliateCampaignId=ePNCampaignId,affiliateReferenceId=referenceId in the header
    in order to be paid for selling eBay items on your site and it is strongly recommended
    you use contextualLocation to improved the estimated delivery window information.
    For details see, Request headers in the Buy APIs Overview. Restrictions For a
    list of supported sites and other restrictions, see API Restrictions. Limitation:
    This call can return a maximum of 10,000 items.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/138-ebay.jpg
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Commerce, Stack, internet, Marketplace, Technology, API Provider, Auctions,
    Profiles, General Data, Relative Data, Service API, Pedestal, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/ebay/item-summarysearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/ebay/item-summarysearch-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://easycron.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ebay.stack.network
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-crunchbase
  url: https://crunchbase.com/organization/leah
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-email
  url: spam@ebay.com
- type: x-email
  url: spoof@ebay.com
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/eBay
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---