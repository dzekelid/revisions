---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API Show revision
  description: Show revision.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/pages/url/revisions:
    get:
      summary: List revisions
      description: List revisions.
      operationId: list-revisions
      x-api-path-slug: groupsgroup-idpagesurlrevisions-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
  /groups/{group_id}/pages/url/revisions/latest:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionslatest-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
      - Latest
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