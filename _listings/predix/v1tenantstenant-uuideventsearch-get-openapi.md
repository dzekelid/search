---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Event Audit Trail Get Tenants Event Search
  description: Get tenants event search.
  version: 1.0.0
host: event-audit-trail.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/tenants/{tenant_uuid}/event-search:
    get:
      summary: Get Tenants Event Search
      description: Get tenants event search.
      operationId: getV1TenantsTenantUuEventSearch
      x-api-path-slug: v1tenantstenant-uuideventsearch-get
      parameters:
      - in: query
        name: query
        description: query
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Event
      - Search
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