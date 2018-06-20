---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/files/{fileId}/revisions:
    get:
      summary: Get Accounts Files Fileid Revisions
      description: Lists other revisions of a given file. Returns a list of revisions
        attached to other emails in the mailbox for a given file. Two files are considered
        revisions of the same document if their file names are identical outside of
        revision indicators such as dates, author initials, version numbers and keywords
        like "final" or "draft".
      operationId: listAccountFileRevisions_
      x-api-path-slug: accountsidfilesfileidrevisions-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Revisions
---