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
  /revisions/{root}/{path}:
    get:
      summary: Obtains metadata for all available revisions of a file, including the
        current revision.
      description: |-
        Obtains metadata for all available revisions of a file, including the current revision.

        Only revisions up to thirty days old are available (or more if the Dropbox user has
        [Extended Version History](https://www.dropbox.com/help/113)). You can use the revision number in conjunction
        with the `/restore` call to revert the file to its previous state.
      operationId: obtains-metadata-for-all-available-revisions-of-a-file-including-the-current-revisiononly-revisions-
      x-api-path-slug: revisionsrootpath-get
      parameters:
      - in: query
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given `locale`
      - in: path
        name: path
        description: The path to the file
      - in: query
        name: rev_limit
        description: Default is 10
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Revisions
      - Root
      - Path
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