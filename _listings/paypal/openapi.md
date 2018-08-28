swagger: "2.0"
x-collection-name: PayPal
x-complete: 1
info:
  title: PayPal (Sandbox)
  description: bring-payments-to-apps-mobile-and-social-with-adaptive-payments-bsandbox-api-b
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Invoice/SearchInvoices:
    post:
      summary: Search Invoices
      description: Use the SearchInvoice API operation to search an invoice.
      operationId: Invoice.SearchInvoices.post
      x-api-path-slug: invoicesearchinvoices-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
      - Search