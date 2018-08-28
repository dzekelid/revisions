---
swagger: "2.0"
x-collection-name: Flat
x-complete: 0
info:
  title: Flat Get a score revision
  description: |-
    When creating a score or saving a new version of a score, a revision is created in our storage. This method allows you to get a specific
    revision metadata.
  termsOfService: https://flat.io/legal
  contact:
    name: Flat
    url: https://flat.io/support
    email: developers@flat.io
  version: 2.1.0
host: api.flat.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scores/{score}/revisions:
    get:
      summary: List the revisions
      description: |-
        When creating a score or saving a new version of a score, a revision is created in our storage. This method allows you to list all of them, sorted by last modification.

        Depending the plan of the account, this list can be trunked to the few last revisions.
      operationId: getScoreRevisions
      x-api-path-slug: scoresscorerevisions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - Revisions
    post:
      summary: Create a new revision
      description: Update a score by uploading a new revision for this one.
      operationId: createScoreRevision
      x-api-path-slug: scoresscorerevisions-post
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
      - New
      - Revision
  /scores/{score}/revisions/{revision}:
    get:
      summary: Get a score revision
      description: |-
        When creating a score or saving a new version of a score, a revision is created in our storage. This method allows you to get a specific
        revision metadata.
      operationId: getScoreRevision
      x-api-path-slug: scoresscorerevisionsrevision-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Score
      - Revision
  /scores/{score}/revisions/{revision}/{format}:
    get:
      summary: Get a score revision data
      description: |-
        Retrieve the file corresponding to a score revision (the following formats are available: Flat JSON/Adagio JSON `json`, MusicXML
        `mxl`/`xml`, MP3 `mp3`, WAV `wav`, MIDI `midi`, or a tumbnail of the first page `thumbnail.png`).
      operationId: getScoreRevisionData
      x-api-path-slug: scoresscorerevisionsrevisionformat-get
      parameters:
      - in: path
        name: format
        description: The format of the file you will retrieve
      - in: query
        name: No Name
      - in: query
        name: onlyCached
        description: Only return files already generated and cached in Flats productioncache
      - in: query
        name: parts
        description: An optional a set of parts to be exported
      responses:
        200:
          description: OK
      tags:
      - Score
      - Revision
      - Data
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