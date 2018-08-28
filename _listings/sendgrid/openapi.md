swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /asm/groups/{group_id}/suppressions/search:
    post:
      summary: Add Asm Groups Group  Suppressions Search
      description: |-
        **This endpoint allows you to search a suppression group for multiple suppressions.**

        When given a list of email addresses and a group ID, this endpoint will return only the email addresses that have been unsubscribed from the given group.

        Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
      operationId: asm.groups.group_id.suppressions.search.post
      x-api-path-slug: asmgroupsgroup-idsuppressionssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
      - ""
      - Suppressions
      - Search
  /contactdb/recipients/search:
    get:
      summary: Get Contactdb Recipients Search
      description: |-
        **This endpoint allows you to perform a search on all of your Marketing Campaigns recipients.**

        field_name:

        * is a variable that is substituted for your actual custom field name from your recipient.
        * Text fields must be url-encoded. Date fields are searchable only by unix timestamp (e.g. 2/2/2015 becomes 1422835200)
        * If field_name is a 'reserved' date field, such as created_at or updated_at, the system will internally convert
        your epoch time to a date range encompassing the entire day. For example, an epoch time of 1422835600 converts to
        Mon, 02 Feb 2015 00:06:40 GMT, but internally the system will search from Mon, 02 Feb 2015 00:00:00 GMT through
        Mon, 02 Feb 2015 23:59:59 GMT.

        The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
      operationId: contactdb.recipients.search.get
      x-api-path-slug: contactdbrecipientssearch-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: '{field_name}'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Search