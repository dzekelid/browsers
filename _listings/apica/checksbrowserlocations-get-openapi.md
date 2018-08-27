---
swagger: "2.0"
x-collection-name: Apica
x-complete: 0
info:
  title: Browser Checks API Checks Browser Locations
  version: 1.0.0
  description: Gets a list of all locations that are available for browser checks.
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/checks/browser ':
    ' post ':
      summary: Checks Browser
      description: Creates a new browser check.
      operationId: -checks-browser-
      x-api-path-slug: checksbrowser-post
      responses:
        200:
          description: OK
      tags:
      - Browser
  '/checks/browser/{checkId} ':
    ' put ':
      summary: Checks Browser
      description: Updates a browser check.
      operationId: -checks-browser-checkid-
      x-api-path-slug: checksbrowsercheckid-put
      responses:
        200:
          description: OK
      tags:
      - Browser
  '/checks/browser/locations ':
    ' get ':
      summary: Checks Browser Locations
      description: Gets a list of all locations that are available for browser checks.
      operationId: -checks-browser-locations-
      x-api-path-slug: checksbrowserlocations-get
      responses:
        200:
          description: OK
      tags:
      - Browser
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