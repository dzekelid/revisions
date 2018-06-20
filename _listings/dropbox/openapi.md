---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox
  description: the-dropbox-api-allows-you-to-build-the-power-of-dropbox-directly-into-your-app-
  version: "1"
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /revisions:
    get:
      summary: Get Revisions
      description: /revisions
      operationId: revisions
      x-api-path-slug: revisions-get
      parameters:
      - in: query
        name: locale
        description: The metadata returned will have its size field translated based
          on the given locale
      - in: query
        name: rev_limit
        description: Default is 10
      responses:
        200:
          description: OK
      tags:
      - Revisions
---