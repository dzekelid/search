swagger: "2.0"
x-collection-name: Digital River
x-complete: 1
info:
  title: Digital River Shopper API
  description: the-dr-connect-shopper-api-operates-on-a-store-and-products-that-are-set-up-in-global-commerce--
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/product-search:
    get:
      summary: Get Shoppers Me Product Search
      description: Get shoppers me product search.
      operationId: getV1ShoppersMeProductSearch
      x-api-path-slug: v1shoppersmeproductsearch-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Product
      - Search
  /v1/shoppers/me/purchase-plan/search:
    get:
      summary: Get Shoppers Me Purchase Plan Search
      description: Get shoppers me purchase plan search.
      operationId: getV1ShoppersMePurchasePlanSearch
      x-api-path-slug: v1shoppersmepurchaseplansearch-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Purchase
      - Plan
      - Search