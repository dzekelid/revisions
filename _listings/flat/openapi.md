---
swagger: "2.0"
x-collection-name: Flat
x-complete: 1
info:
  title: Flat
  description: the-flat-api-allows-you-to-easily-extend-the-abilities-of-the-flat-platformhttpsflat-io-with-a-wide-range-of-use-cases-including-the-following-creating-and-importing-new-music-scores-using-musicxml-or-midi-files--browsing-updating-copying-exporting-the-users-scores-for-example-in-mp3-wav-or-midi--managing-educational-resources-with-flat-for-education-creating--updating-the-organization-accounts-the-classes-rosters-and-assignments--the-flat-api-is-built-on-http--our-api-is-restful-it-has-predictable-resource-urls--it-returns-http-response-codes-to-indicate-errors--it-also-accepts-and-returns-json-in-the-http-body--
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
---