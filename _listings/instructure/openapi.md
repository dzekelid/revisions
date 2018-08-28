swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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
  /courses/{course_id}/pages/url/revisions:
    get:
      summary: List revisions
      description: List revisions.
      operationId: list-revisions
      x-api-path-slug: coursescourse-idpagesurlrevisions-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
      - Revisions
  /courses/{course_id}/pages/url/revisions/latest:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: coursescourse-idpagesurlrevisionslatest-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
      - Revisions
      - Latest
  /courses/{course_id}/pages/url/revisions/{revision_id}:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: coursescourse-idpagesurlrevisionsrevision-id-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
      - Revisions
      - Revision
      - Id
    post:
      summary: Revert to revision
      description: Revert to revision.
      operationId: revert-to-revision
      x-api-path-slug: coursescourse-idpagesurlrevisionsrevision-id-post
      parameters:
      - in: query
        name: revision_id
        description: The revision to revert to (use the List Revisions API to see
          available revisions)
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
      - Revisions
      - Revision
      - Id
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
  /groups/{group_id}/pages/url/revisions/{revision_id}:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionsrevision-id-get
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
      - Revision
      - Id
    post:
      summary: Revert to revision
      description: Revert to revision.
      operationId: revert-to-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionsrevision-id-post
      parameters:
      - in: query
        name: revision_id
        description: The revision to revert to (use the List Revisions API to see
          available revisions)
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
      - Revision
      - Id