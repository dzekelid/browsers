swagger: "2.0"
x-collection-name: Browshot
x-complete: 1
info:
  title: Browshot
  description: take-screenshots-of-any-website-in-real-time
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /browser/info:
    get:
      summary: Get information about a browser
      description: Get information about a browser.
      operationId: GetBrowserInfo
      x-api-path-slug: browserinfo-get
      parameters:
      - in: query
        name: id
        description: browser ID
      responses:
        200:
          description: OK
      tags:
      - Browser
      - Info
  /browser/list:
    get:
      summary: Get all browsers
      description: Get all browsers.
      operationId: GetBrowsersInfo
      x-api-path-slug: browserlist-get
      responses:
        200:
          description: OK
      tags:
      - Browser
      - List