---
swagger: "2.0"
x-collection-name: Google Drive
x-complete: 0
info:
  title: Google Drive Delete File Revision
  description: Permanently deletes a revision. This method is only applicable to files
    with binary content in Drive.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /drive/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{fileId}/revisions:
    get:
      summary: Get File Revisions
      description: Lists a file's revisions.
      operationId: drive.revisions.list
      x-api-path-slug: filesfileidrevisions-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: pageSize
        description: The maximum number of revisions to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      responses:
        200:
          description: OK
      tags:
      - Revision
  /files/{fileId}/revisions/{revisionId}:
    delete:
      summary: Delete File Revision
      description: Permanently deletes a revision. This method is only applicable
        to files with binary content in Drive.
      operationId: drive.revisions.delete
      x-api-path-slug: filesfileidrevisionsrevisionid-delete
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: revisionId
        description: The ID of the revision
      responses:
        200:
          description: OK
      tags:
      - Revision
    get:
      summary: Get File Revision
      description: Gets a revision's metadata or content by ID.
      operationId: drive.revisions.get
      x-api-path-slug: filesfileidrevisionsrevisionid-get
      parameters:
      - in: query
        name: acknowledgeAbuse
        description: Whether the user is acknowledging the risk of downloading known
          malware or other abusive files
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: revisionId
        description: The ID of the revision
      responses:
        200:
          description: OK
      tags:
      - Revision
    patch:
      summary: Update File Revision
      description: Updates a revision with patch semantics.
      operationId: drive.revisions.update
      x-api-path-slug: filesfileidrevisionsrevisionid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: revisionId
        description: The ID of the revision
      responses:
        200:
          description: OK
      tags:
      - Revision
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