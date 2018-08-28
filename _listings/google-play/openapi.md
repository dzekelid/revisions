swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /revisions/check:
    get:
      summary: Check Revision
      description: Checks whether the games client is out of date.
      operationId: games.revisions.check
      x-api-path-slug: revisionscheck-get
      parameters:
      - in: query
        name: clientRevision
        description: The revision of the client SDK used by your application
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Revision