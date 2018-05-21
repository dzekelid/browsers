---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  description: the-sendgrid-web-api-v3-documentation-this-is-the-entirety-of-the-documented-v3-endpoints-we-have-updated-all-the-descriptions-parameters-requests-and-responses-authentication-every-endpoint-requires-authentication-in-the-form-of-an-authorization-header-authorization-bearer-api-key
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
  /browsers/stats:
    get:
      summary: Get Browsers Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by browser type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: browsers.stats.get
      x-api-path-slug: browsersstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the stats
      - in: query
        name: browsers
        description: The browsers to get statistics for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include on each page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to exclude
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Browsers
      - Stats
---