---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Datastore API Get Revisions
  description: /revisions
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