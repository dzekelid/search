---
swagger: "2.0"
info:
  title: Square Connect API Post V2 Catalog Search
  description: |-
    Queries the targeted catalog using a variety of query types:
    [CatalogQuerySortedAttribute](#type-catalogquerysortedattribute),
    [CatalogQueryExact](#type-catalogqueryexact),
    [CatalogQueryRange](#type-catalogqueryrange),
    [CatalogQueryText](#type-catalogquerytext),
    [CatalogQueryItemsForTax](#type-catalogqueryitemsfortax), and
    [CatalogQueryItemsForModifierList](#type-catalogqueryitemsformodifierlist).
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: 1.0.0
host: connect.squareup.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/catalog/search:
    post:
      summary: Post V2 Catalog Search
      description: |-
        Queries the targeted catalog using a variety of query types:
        [CatalogQuerySortedAttribute](#type-catalogquerysortedattribute),
        [CatalogQueryExact](#type-catalogqueryexact),
        [CatalogQueryRange](#type-catalogqueryrange),
        [CatalogQueryText](#type-catalogquerytext),
        [CatalogQueryItemsForTax](#type-catalogqueryitemsfortax), and
        [CatalogQueryItemsForModifierList](#type-catalogqueryitemsformodifierlist)
      operationId: postV2CatalogSearch
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - catalog
      - search
definitions:
  AdditionalRecipient:
    properties:
      location_id:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
      receivable_id:
        description: This is a default description.
        type: delete
  AdditionalRecipientReceivable:
    properties:
      id:
        description: This is a default description.
        type: delete
      transaction_id:
        description: This is a default description.
        type: delete
      transaction_location_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      refunds:
        description: This is a default description.
        type: delete
  AdditionalRecipientReceivableRefund:
    properties:
      id:
        description: This is a default description.
        type: delete
      receivable_id:
        description: This is a default description.
        type: delete
      refund_id:
        description: This is a default description.
        type: delete
      transaction_location_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
  Address:
    properties:
      address_line_1:
        description: This is a default description.
        type: delete
      address_line_2:
        description: This is a default description.
        type: delete
      address_line_3:
        description: This is a default description.
        type: delete
      locality:
        description: This is a default description.
        type: delete
      sublocality:
        description: This is a default description.
        type: delete
      sublocality_2:
        description: This is a default description.
        type: delete
      sublocality_3:
        description: This is a default description.
        type: delete
      administrative_district_level_1:
        description: This is a default description.
        type: delete
      administrative_district_level_2:
        description: This is a default description.
        type: delete
      administrative_district_level_3:
        description: This is a default description.
        type: delete
  BatchDeleteCatalogObjectsRequest:
    properties:
      object_ids:
        description: This is a default description.
        type: delete
  BatchDeleteCatalogObjectsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      deleted_object_ids:
        description: This is a default description.
        type: delete
      deleted_at:
        description: This is a default description.
        type: delete
  BatchRetrieveCatalogObjectsRequest:
    properties:
      object_ids:
        description: This is a default description.
        type: delete
      include_related_objects:
        description: This is a default description.
        type: delete
  BatchRetrieveCatalogObjectsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      objects:
        description: This is a default description.
        type: delete
      related_objects:
        description: This is a default description.
        type: delete
  BatchRetrieveOrdersRequest:
    properties:
      order_ids:
        description: This is a default description.
        type: delete
  BatchRetrieveOrdersResponse:
    properties:
      orders:
        description: This is a default description.
        type: delete
      errors:
        description: This is a default description.
        type: delete
  BatchUpsertCatalogObjectsRequest:
    properties:
      idempotency_key:
        description: This is a default description.
        type: delete
      batches:
        description: This is a default description.
        type: delete
  BatchUpsertCatalogObjectsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      objects:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
      id_mappings:
        description: This is a default description.
        type: delete
  CaptureTransactionRequest:
    properties: []
  CaptureTransactionResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  Card:
    properties:
      id:
        description: This is a default description.
        type: delete
      card_brand:
        description: This is a default description.
        type: delete
      last_4:
        description: This is a default description.
        type: delete
      exp_month:
        description: This is a default description.
        type: delete
      exp_year:
        description: This is a default description.
        type: delete
      cardholder_name:
        description: This is a default description.
        type: delete
      fingerprint:
        description: This is a default description.
        type: delete
  CatalogCategory:
    properties:
      name:
        description: This is a default description.
        type: delete
  CatalogDiscount:
    properties:
      name:
        description: This is a default description.
        type: delete
      discount_type:
        description: This is a default description.
        type: delete
      percentage:
        description: This is a default description.
        type: delete
      pin_required:
        description: This is a default description.
        type: delete
      label_color:
        description: This is a default description.
        type: delete
  CatalogIdMapping:
    properties:
      client_object_id:
        description: This is a default description.
        type: delete
      object_id:
        description: This is a default description.
        type: delete
  CatalogInfoRequest:
    properties: []
  CatalogInfoResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  CatalogInfoResponseLimits:
    properties:
      batch_upsert_max_objects_per_batch:
        description: This is a default description.
        type: delete
      batch_upsert_max_total_objects:
        description: This is a default description.
        type: delete
      batch_retrieve_max_object_ids:
        description: This is a default description.
        type: delete
      search_max_page_limit:
        description: This is a default description.
        type: delete
      batch_delete_max_object_ids:
        description: This is a default description.
        type: delete
      update_item_taxes_max_item_ids:
        description: This is a default description.
        type: delete
      update_item_taxes_max_taxes_to_enable:
        description: This is a default description.
        type: delete
      update_item_taxes_max_taxes_to_disable:
        description: This is a default description.
        type: delete
      update_item_modifier_lists_max_item_ids:
        description: This is a default description.
        type: delete
      update_item_modifier_lists_max_modifier_lists_to_enable:
        description: This is a default description.
        type: delete
  CatalogItem:
    properties:
      name:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
      abbreviation:
        description: This is a default description.
        type: delete
      label_color:
        description: This is a default description.
        type: delete
      available_online:
        description: This is a default description.
        type: delete
      available_for_pickup:
        description: This is a default description.
        type: delete
      available_electronically:
        description: This is a default description.
        type: delete
      category_id:
        description: This is a default description.
        type: delete
      tax_ids:
        description: This is a default description.
        type: delete
      modifier_list_info:
        description: This is a default description.
        type: delete
  CatalogItemModifierListInfo:
    properties:
      modifier_list_id:
        description: This is a default description.
        type: delete
      modifier_overrides:
        description: This is a default description.
        type: delete
      min_selected_modifiers:
        description: This is a default description.
        type: delete
      max_selected_modifiers:
        description: This is a default description.
        type: delete
      enabled:
        description: This is a default description.
        type: delete
  CatalogItemVariation:
    properties:
      item_id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      sku:
        description: This is a default description.
        type: delete
      upc:
        description: This is a default description.
        type: delete
      ordinal:
        description: This is a default description.
        type: delete
      pricing_type:
        description: This is a default description.
        type: delete
      location_overrides:
        description: This is a default description.
        type: delete
      track_inventory:
        description: This is a default description.
        type: delete
      inventory_alert_type:
        description: This is a default description.
        type: delete
      inventory_alert_threshold:
        description: This is a default description.
        type: delete
  CatalogModifier:
    properties:
      name:
        description: This is a default description.
        type: delete
  CatalogModifierList:
    properties:
      name:
        description: This is a default description.
        type: delete
      selection_type:
        description: This is a default description.
        type: delete
      modifiers:
        description: This is a default description.
        type: delete
  CatalogModifierOverride:
    properties:
      modifier_id:
        description: This is a default description.
        type: delete
      on_by_default:
        description: This is a default description.
        type: delete
  CatalogObject:
    properties:
      type:
        description: This is a default description.
        type: delete
      id:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
      version:
        description: This is a default description.
        type: delete
      is_deleted:
        description: This is a default description.
        type: delete
      catalog_v1_ids:
        description: This is a default description.
        type: delete
      present_at_all_locations:
        description: This is a default description.
        type: delete
      present_at_location_ids:
        description: This is a default description.
        type: delete
      absent_at_location_ids:
        description: This is a default description.
        type: delete
  CatalogObjectBatch:
    properties:
      objects:
        description: This is a default description.
        type: delete
  CatalogQuery:
    properties: []
  CatalogQueryExact:
    properties:
      attribute_name:
        description: This is a default description.
        type: delete
      attribute_value:
        description: This is a default description.
        type: delete
  CatalogQueryItemsForModifierList:
    properties:
      modifier_list_ids:
        description: This is a default description.
        type: delete
  CatalogQueryItemsForTax:
    properties:
      tax_ids:
        description: This is a default description.
        type: delete
  CatalogQueryPrefix:
    properties:
      attribute_name:
        description: This is a default description.
        type: delete
      attribute_prefix:
        description: This is a default description.
        type: delete
  CatalogQueryRange:
    properties:
      attribute_name:
        description: This is a default description.
        type: delete
      attribute_min_value:
        description: This is a default description.
        type: delete
      attribute_max_value:
        description: This is a default description.
        type: delete
  CatalogQuerySortedAttribute:
    properties:
      attribute_name:
        description: This is a default description.
        type: delete
      initial_attribute_value:
        description: This is a default description.
        type: delete
      sort_order:
        description: This is a default description.
        type: delete
  CatalogQueryText:
    properties:
      keywords:
        description: This is a default description.
        type: delete
  CatalogTax:
    properties:
      name:
        description: This is a default description.
        type: delete
      calculation_phase:
        description: This is a default description.
        type: delete
      inclusion_type:
        description: This is a default description.
        type: delete
      percentage:
        description: This is a default description.
        type: delete
      applies_to_custom_amounts:
        description: This is a default description.
        type: delete
      enabled:
        description: This is a default description.
        type: delete
  CatalogV1Id:
    properties:
      catalog_v1_id:
        description: This is a default description.
        type: delete
      location_id:
        description: This is a default description.
        type: delete
  ChargeRequest:
    properties:
      idempotency_key:
        description: This is a default description.
        type: delete
      card_nonce:
        description: This is a default description.
        type: delete
      customer_card_id:
        description: This is a default description.
        type: delete
      delay_capture:
        description: This is a default description.
        type: delete
      reference_id:
        description: This is a default description.
        type: delete
      note:
        description: This is a default description.
        type: delete
      customer_id:
        description: This is a default description.
        type: delete
      buyer_email_address:
        description: This is a default description.
        type: delete
      order_id:
        description: This is a default description.
        type: delete
      additional_recipients:
        description: This is a default description.
        type: delete
  ChargeRequestAdditionalRecipient:
    properties:
      location_id:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  ChargeResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  Checkout:
    properties:
      id:
        description: This is a default description.
        type: delete
      checkout_page_url:
        description: This is a default description.
        type: delete
      ask_for_shipping_address:
        description: This is a default description.
        type: delete
      merchant_support_email:
        description: This is a default description.
        type: delete
      pre_populate_buyer_email:
        description: This is a default description.
        type: delete
      redirect_url:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      additional_recipients:
        description: This is a default description.
        type: delete
  CreateCheckoutRequest:
    properties:
      idempotency_key:
        description: This is a default description.
        type: delete
      ask_for_shipping_address:
        description: This is a default description.
        type: delete
      merchant_support_email:
        description: This is a default description.
        type: delete
      pre_populate_buyer_email:
        description: This is a default description.
        type: delete
      redirect_url:
        description: This is a default description.
        type: delete
      additional_recipients:
        description: This is a default description.
        type: delete
  CreateCheckoutResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  CreateCustomerCardRequest:
    properties:
      card_nonce:
        description: This is a default description.
        type: delete
      cardholder_name:
        description: This is a default description.
        type: delete
  CreateCustomerCardResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  CreateCustomerRequest:
    properties:
      given_name:
        description: This is a default description.
        type: delete
      family_name:
        description: This is a default description.
        type: delete
      company_name:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      email_address:
        description: This is a default description.
        type: delete
      phone_number:
        description: This is a default description.
        type: delete
      reference_id:
        description: This is a default description.
        type: delete
      note:
        description: This is a default description.
        type: delete
  CreateCustomerResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  CreateOrderRequest:
    properties:
      idempotency_key:
        description: This is a default description.
        type: delete
      reference_id:
        description: This is a default description.
        type: delete
      line_items:
        description: This is a default description.
        type: delete
      taxes:
        description: This is a default description.
        type: delete
      discounts:
        description: This is a default description.
        type: delete
  CreateOrderRequestDiscount:
    properties:
      catalog_object_id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      percentage:
        description: This is a default description.
        type: delete
  CreateOrderRequestLineItem:
    properties:
      name:
        description: This is a default description.
        type: delete
      quantity:
        description: This is a default description.
        type: delete
      variation_name:
        description: This is a default description.
        type: delete
      note:
        description: This is a default description.
        type: delete
      catalog_object_id:
        description: This is a default description.
        type: delete
      modifiers:
        description: This is a default description.
        type: delete
      taxes:
        description: This is a default description.
        type: delete
      discounts:
        description: This is a default description.
        type: delete
  CreateOrderRequestModifier:
    properties:
      catalog_object_id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
  CreateOrderRequestTax:
    properties:
      catalog_object_id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      percentage:
        description: This is a default description.
        type: delete
  CreateOrderResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  CreateRefundRequest:
    properties:
      idempotency_key:
        description: This is a default description.
        type: delete
      tender_id:
        description: This is a default description.
        type: delete
      reason:
        description: This is a default description.
        type: delete
  CreateRefundResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  Customer:
    properties:
      id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
      cards:
        description: This is a default description.
        type: delete
      given_name:
        description: This is a default description.
        type: delete
      family_name:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      company_name:
        description: This is a default description.
        type: delete
      email_address:
        description: This is a default description.
        type: delete
      phone_number:
        description: This is a default description.
        type: delete
  CustomerGroupInfo:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
  CustomerPreferences:
    properties:
      email_unsubscribed:
        description: This is a default description.
        type: delete
  DeleteCatalogObjectRequest:
    properties: []
  DeleteCatalogObjectResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      deleted_object_ids:
        description: This is a default description.
        type: delete
      deleted_at:
        description: This is a default description.
        type: delete
  DeleteCustomerCardRequest:
    properties: []
  DeleteCustomerCardResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  DeleteCustomerRequest:
    properties: []
  DeleteCustomerResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  Error:
    properties:
      category:
        description: This is a default description.
        type: delete
      code:
        description: This is a default description.
        type: delete
      detail:
        description: This is a default description.
        type: delete
      field:
        description: This is a default description.
        type: delete
  ItemVariationLocationOverrides:
    properties:
      location_id:
        description: This is a default description.
        type: delete
      pricing_type:
        description: This is a default description.
        type: delete
      track_inventory:
        description: This is a default description.
        type: delete
      inventory_alert_type:
        description: This is a default description.
        type: delete
      inventory_alert_threshold:
        description: This is a default description.
        type: delete
  ListAdditionalRecipientReceivableRefundsRequest:
    properties:
      begin_time:
        description: This is a default description.
        type: delete
      end_time:
        description: This is a default description.
        type: delete
      sort_order:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListAdditionalRecipientReceivableRefundsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      receivable_refunds:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListAdditionalRecipientReceivablesRequest:
    properties:
      begin_time:
        description: This is a default description.
        type: delete
      end_time:
        description: This is a default description.
        type: delete
      sort_order:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListAdditionalRecipientReceivablesResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      receivables:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListCatalogRequest:
    properties:
      cursor:
        description: This is a default description.
        type: delete
      types:
        description: This is a default description.
        type: delete
  ListCatalogResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
      objects:
        description: This is a default description.
        type: delete
  ListCustomersRequest:
    properties:
      cursor:
        description: This is a default description.
        type: delete
  ListCustomersResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      customers:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListLocationsRequest:
    properties: []
  ListLocationsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      locations:
        description: This is a default description.
        type: delete
  ListRefundsRequest:
    properties:
      begin_time:
        description: This is a default description.
        type: delete
      end_time:
        description: This is a default description.
        type: delete
      sort_order:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListRefundsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      refunds:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListTransactionsRequest:
    properties:
      begin_time:
        description: This is a default description.
        type: delete
      end_time:
        description: This is a default description.
        type: delete
      sort_order:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  ListTransactionsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      transactions:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
  Location:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      timezone:
        description: This is a default description.
        type: delete
      capabilities:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      merchant_id:
        description: This is a default description.
        type: delete
      country:
        description: This is a default description.
        type: delete
      language_code:
        description: This is a default description.
        type: delete
      currency:
        description: This is a default description.
        type: delete
  Money:
    properties:
      amount:
        description: This is a default description.
        type: delete
      currency:
        description: This is a default description.
        type: delete
  Order:
    properties:
      id:
        description: This is a default description.
        type: delete
      location_id:
        description: This is a default description.
        type: delete
      reference_id:
        description: This is a default description.
        type: delete
      line_items:
        description: This is a default description.
        type: delete
  OrderLineItem:
    properties:
      name:
        description: This is a default description.
        type: delete
      quantity:
        description: This is a default description.
        type: delete
      note:
        description: This is a default description.
        type: delete
      catalog_object_id:
        description: This is a default description.
        type: delete
      variation_name:
        description: This is a default description.
        type: delete
      modifiers:
        description: This is a default description.
        type: delete
      taxes:
        description: This is a default description.
        type: delete
      discounts:
        description: This is a default description.
        type: delete
  OrderLineItemDiscount:
    properties:
      catalog_object_id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      percentage:
        description: This is a default description.
        type: delete
      scope:
        description: This is a default description.
        type: delete
  OrderLineItemModifier:
    properties:
      catalog_object_id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
  OrderLineItemTax:
    properties:
      catalog_object_id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      percentage:
        description: This is a default description.
        type: delete
  Refund:
    properties:
      id:
        description: This is a default description.
        type: delete
      location_id:
        description: This is a default description.
        type: delete
      transaction_id:
        description: This is a default description.
        type: delete
      tender_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      reason:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      additional_recipients:
        description: This is a default description.
        type: delete
  RegisterDomainRequest:
    properties:
      domain_name:
        description: This is a default description.
        type: delete
  RegisterDomainResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
  RetrieveCatalogObjectRequest:
    properties:
      include_related_objects:
        description: This is a default description.
        type: delete
  RetrieveCatalogObjectResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      related_objects:
        description: This is a default description.
        type: delete
  RetrieveCustomerRequest:
    properties: []
  RetrieveCustomerResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  RetrieveTransactionRequest:
    properties: []
  RetrieveTransactionResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  SearchCatalogObjectsRequest:
    properties:
      cursor:
        description: This is a default description.
        type: delete
      object_types:
        description: This is a default description.
        type: delete
      include_deleted_objects:
        description: This is a default description.
        type: delete
      include_related_objects:
        description: This is a default description.
        type: delete
      begin_time:
        description: This is a default description.
        type: delete
      limit:
        description: This is a default description.
        type: delete
  SearchCatalogObjectsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      cursor:
        description: This is a default description.
        type: delete
      objects:
        description: This is a default description.
        type: delete
      related_objects:
        description: This is a default description.
        type: delete
  Tender:
    properties:
      id:
        description: This is a default description.
        type: delete
      location_id:
        description: This is a default description.
        type: delete
      transaction_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      note:
        description: This is a default description.
        type: delete
      customer_id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      additional_recipients:
        description: This is a default description.
        type: delete
  TenderCardDetails:
    properties:
      status:
        description: This is a default description.
        type: delete
      entry_method:
        description: This is a default description.
        type: delete
  TenderCashDetails:
    properties: []
  Transaction:
    properties:
      id:
        description: This is a default description.
        type: delete
      location_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      tenders:
        description: This is a default description.
        type: delete
      refunds:
        description: This is a default description.
        type: delete
      reference_id:
        description: This is a default description.
        type: delete
      product:
        description: This is a default description.
        type: delete
      client_id:
        description: This is a default description.
        type: delete
      order_id:
        description: This is a default description.
        type: delete
  UpdateCustomerRequest:
    properties:
      given_name:
        description: This is a default description.
        type: delete
      family_name:
        description: This is a default description.
        type: delete
      company_name:
        description: This is a default description.
        type: delete
      nickname:
        description: This is a default description.
        type: delete
      email_address:
        description: This is a default description.
        type: delete
      phone_number:
        description: This is a default description.
        type: delete
      reference_id:
        description: This is a default description.
        type: delete
      note:
        description: This is a default description.
        type: delete
  UpdateCustomerResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  UpdateItemModifierListsRequest:
    properties:
      item_ids:
        description: This is a default description.
        type: delete
      modifier_lists_to_enable:
        description: This is a default description.
        type: delete
      modifier_lists_to_disable:
        description: This is a default description.
        type: delete
  UpdateItemModifierListsResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
  UpdateItemTaxesRequest:
    properties:
      item_ids:
        description: This is a default description.
        type: delete
      taxes_to_enable:
        description: This is a default description.
        type: delete
      taxes_to_disable:
        description: This is a default description.
        type: delete
  UpdateItemTaxesResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
  UpsertCatalogObjectRequest:
    properties:
      idempotency_key:
        description: This is a default description.
        type: delete
  UpsertCatalogObjectResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
      id_mappings:
        description: This is a default description.
        type: delete
  VoidTransactionRequest:
    properties: []
  VoidTransactionResponse:
    properties:
      errors:
        description: This is a default description.
        type: delete
  v1Money:
    properties:
      amount:
        description: This is a default description.
        type: delete
      currency_code:
        description: This is a default description.
        type: delete
  v1PhoneNumber:
    properties:
      calling_code:
        description: This is a default description.
        type: delete
      number:
        description: This is a default description.
        type: delete
  v1Merchant:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      email:
        description: This is a default description.
        type: delete
      account_type:
        description: This is a default description.
        type: delete
      account_capabilities:
        description: This is a default description.
        type: delete
      country_code:
        description: This is a default description.
        type: delete
      language_code:
        description: This is a default description.
        type: delete
      currency_code:
        description: This is a default description.
        type: delete
      business_name:
        description: This is a default description.
        type: delete
      business_type:
        description: This is a default description.
        type: delete
  v1Employee:
    properties:
      id:
        description: This is a default description.
        type: delete
      first_name:
        description: This is a default description.
        type: delete
      last_name:
        description: This is a default description.
        type: delete
      role_ids:
        description: This is a default description.
        type: delete
      authorized_location_ids:
        description: This is a default description.
        type: delete
      email:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      external_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
  v1EmployeeRole:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      permissions:
        description: This is a default description.
        type: delete
      is_owner:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
  v1Timecard:
    properties:
      id:
        description: This is a default description.
        type: delete
      employee_id:
        description: This is a default description.
        type: delete
      deleted:
        description: This is a default description.
        type: delete
      clockin_time:
        description: This is a default description.
        type: delete
      clockout_time:
        description: This is a default description.
        type: delete
      clockin_location_id:
        description: This is a default description.
        type: delete
      clockout_location_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
  v1TimecardEvent:
    properties:
      id:
        description: This is a default description.
        type: delete
      event_type:
        description: This is a default description.
        type: delete
      clockin_time:
        description: This is a default description.
        type: delete
      clockout_time:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
  Device:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
  v1CashDrawerEvent:
    properties:
      id:
        description: This is a default description.
        type: delete
      employee_id:
        description: This is a default description.
        type: delete
      event_type:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  v1CashDrawerShift:
    properties:
      id:
        description: This is a default description.
        type: delete
      event_type:
        description: This is a default description.
        type: delete
      opened_at:
        description: This is a default description.
        type: delete
      ended_at:
        description: This is a default description.
        type: delete
      closed_at:
        description: This is a default description.
        type: delete
      employee_ids:
        description: This is a default description.
        type: delete
      opening_employee_id:
        description: This is a default description.
        type: delete
      ending_employee_id:
        description: This is a default description.
        type: delete
      closing_employee_id:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
  v1Payment:
    properties:
      id:
        description: This is a default description.
        type: delete
      merchant_id:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      creator_id:
        description: This is a default description.
        type: delete
      payment_url:
        description: This is a default description.
        type: delete
      receipt_url:
        description: This is a default description.
        type: delete
      inclusive_tax:
        description: This is a default description.
        type: delete
      additive_tax:
        description: This is a default description.
        type: delete
      tender:
        description: This is a default description.
        type: delete
      refunds:
        description: This is a default description.
        type: delete
  v1PaymentItemization:
    properties:
      name:
        description: This is a default description.
        type: delete
      quantity:
        description: This is a default description.
        type: delete
      itemization_type:
        description: This is a default description.
        type: delete
      notes:
        description: This is a default description.
        type: delete
      item_variation_name:
        description: This is a default description.
        type: delete
      taxes:
        description: This is a default description.
        type: delete
      discounts:
        description: This is a default description.
        type: delete
      modifiers:
        description: This is a default description.
        type: delete
  v1PaymentModifier:
    properties:
      name:
        description: This is a default description.
        type: delete
      modifier_option_id:
        description: This is a default description.
        type: delete
  v1PaymentDiscount:
    properties:
      name:
        description: This is a default description.
        type: delete
      discount_id:
        description: This is a default description.
        type: delete
  v1PaymentItemDetail:
    properties:
      category_name:
        description: This is a default description.
        type: delete
      sku:
        description: This is a default description.
        type: delete
      item_id:
        description: This is a default description.
        type: delete
      item_variation_id:
        description: This is a default description.
        type: delete
  v1Refund:
    properties:
      type:
        description: This is a default description.
        type: delete
      reason:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      processed_at:
        description: This is a default description.
        type: delete
      payment_id:
        description: This is a default description.
        type: delete
      merchant_id:
        description: This is a default description.
        type: delete
      is_exchange:
        description: This is a default description.
        type: delete
  v1Settlement:
    properties:
      id:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      initiated_at:
        description: This is a default description.
        type: delete
      bank_account_id:
        description: This is a default description.
        type: delete
      entries:
        description: This is a default description.
        type: delete
  v1SettlementEntry:
    properties:
      payment_id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
  v1Tender:
    properties:
      id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      employee_id:
        description: This is a default description.
        type: delete
      receipt_url:
        description: This is a default description.
        type: delete
      card_brand:
        description: This is a default description.
        type: delete
      pan_suffix:
        description: This is a default description.
        type: delete
      entry_method:
        description: This is a default description.
        type: delete
      payment_note:
        description: This is a default description.
        type: delete
      is_exchange:
        description: This is a default description.
        type: delete
  v1PaymentTax:
    properties:
      errors:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      rate:
        description: This is a default description.
        type: delete
      inclusion_type:
        description: This is a default description.
        type: delete
      fee_id:
        description: This is a default description.
        type: delete
  v1Order:
    properties:
      errors:
        description: This is a default description.
        type: delete
      id:
        description: This is a default description.
        type: delete
      buyer_email:
        description: This is a default description.
        type: delete
      recipient_name:
        description: This is a default description.
        type: delete
      recipient_phone_number:
        description: This is a default description.
        type: delete
      state:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
      updated_at:
        description: This is a default description.
        type: delete
      expires_at:
        description: This is a default description.
        type: delete
      payment_id:
        description: This is a default description.
        type: delete
  v1OrderHistoryEntry:
    properties:
      action:
        description: This is a default description.
        type: delete
      created_at:
        description: This is a default description.
        type: delete
  v1BankAccount:
    properties:
      id:
        description: This is a default description.
        type: delete
      merchant_id:
        description: This is a default description.
        type: delete
      bank_name:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      routing_number:
        description: This is a default description.
        type: delete
      account_number_suffix:
        description: This is a default description.
        type: delete
      currency_code:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
  v1Variation:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      item_id:
        description: This is a default description.
        type: delete
      ordinal:
        description: This is a default description.
        type: delete
      pricing_type:
        description: This is a default description.
        type: delete
      sku:
        description: This is a default description.
        type: delete
      track_inventory:
        description: This is a default description.
        type: delete
      inventory_alert_type:
        description: This is a default description.
        type: delete
      inventory_alert_threshold:
        description: This is a default description.
        type: delete
      user_data:
        description: This is a default description.
        type: delete
  v1Item:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      color:
        description: This is a default description.
        type: delete
      abbreviation:
        description: This is a default description.
        type: delete
      visibility:
        description: This is a default description.
        type: delete
      available_online:
        description: This is a default description.
        type: delete
      variations:
        description: This is a default description.
        type: delete
      modifier_lists:
        description: This is a default description.
        type: delete
  v1Fee:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      rate:
        description: This is a default description.
        type: delete
      calculation_phase:
        description: This is a default description.
        type: delete
      adjustment_type:
        description: This is a default description.
        type: delete
      applies_to_custom_amounts:
        description: This is a default description.
        type: delete
      enabled:
        description: This is a default description.
        type: delete
      inclusion_type:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
  v1ModifierList:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      selection_type:
        description: This is a default description.
        type: delete
      modifier_options:
        description: This is a default description.
        type: delete
  v1ModifierOption:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      on_by_default:
        description: This is a default description.
        type: delete
      ordinal:
        description: This is a default description.
        type: delete
      modifier_list_id:
        description: This is a default description.
        type: delete
  v1Category:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
  v1ItemImage:
    properties:
      id:
        description: This is a default description.
        type: delete
      url:
        description: This is a default description.
        type: delete
  v1InventoryEntry:
    properties:
      variation_id:
        description: This is a default description.
        type: delete
      quantity_on_hand:
        description: This is a default description.
        type: delete
  v1AdjustInventoryRequest:
    properties:
      quantity_delta:
        description: This is a default description.
        type: delete
      adjustment_type:
        description: This is a default description.
        type: delete
      memo:
        description: This is a default description.
        type: delete
  v1Discount:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      rate:
        description: This is a default description.
        type: delete
      discount_type:
        description: This is a default description.
        type: delete
      pin_required:
        description: This is a default description.
        type: delete
      color:
        description: This is a default description.
        type: delete
  v1Page:
    properties:
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      page_index:
        description: This is a default description.
        type: delete
      cells:
        description: This is a default description.
        type: delete
  v1PageCell:
    properties:
      page_id:
        description: This is a default description.
        type: delete
      row:
        description: This is a default description.
        type: delete
      column:
        description: This is a default description.
        type: delete
      object_type:
        description: This is a default description.
        type: delete
      object_id:
        description: This is a default description.
        type: delete
      placeholder_type:
        description: This is a default description.
        type: delete
  v1CreateRefundRequest:
    properties:
      payment_id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      reason:
        description: This is a default description.
        type: delete
      request_idempotence_key:
        description: This is a default description.
        type: delete
  v1UpdateOrderRequest:
    properties:
      action:
        description: This is a default description.
        type: delete
      shipped_tracking_number:
        description: This is a default description.
        type: delete
      completed_note:
        description: This is a default description.
        type: delete
      refunded_note:
        description: This is a default description.
        type: delete
      canceled_note:
        description: This is a default description.
        type: delete
  v1UpdateModifierListRequest:
    properties:
      name:
        description: This is a default description.
        type: delete
      selection_type:
        description: This is a default description.
        type: delete
x-collection-name: Square
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