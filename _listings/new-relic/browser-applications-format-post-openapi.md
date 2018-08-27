---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Add Browser Applications. Format
  version: 1.0.0
  description: This API endpoint allows you to create a standalone Browser Application.
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /browser_applications.{format}:
    get:
      summary: Get Browser Applications. Format
      description: |-
        This API endpoint returns a list of the Browser Applications associated with your New Relic account.

        Browser Applications can be filtered by their name, or by the application IDs.
      operationId: getBrowserApplications.Format
      x-api-path-slug: browser-applications-format-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter by application ids
        type: list
      - in: query
        name: filter[name]
        description: Filter by application name
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Browser
      - Applications.
      - Format
    post:
      summary: Add Browser Applications. Format
      description: This API endpoint allows you to create a standalone Browser Application.
      operationId: postBrowserApplications.Format
      x-api-path-slug: browser-applications-format-post
      parameters:
      - in: body
        name: browser_application
        description: Browser Application Schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Browser
      - Applications.
      - Format
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