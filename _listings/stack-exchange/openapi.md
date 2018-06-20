---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/{ids}/revisions:
    get:
      summary: Get Post Revisions
      description: "Returns edit revisions for the posts identified in ids.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for post_id, answer_id, or question_id on post, answer, and question
        objects respectively.\n \nThis method returns a list of revisions."
      operationId: returns-edit-revisions-for-the-posts-identified-in-ids-ids-can-contain-up-to-100-semicolon-delimited
      x-api-path-slug: postsidsrevisions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Revisions
  /revisions/{ids}:
    get:
      summary: Get Revisions
      description: "Returns edit revisions identified by ids in {ids}.\n \n{ids} can
        contain up to 20 semicolon delimited ids, to find ids programatically look
        for revision_guid on revision objects. Note that unlike most other id types
        in the API, revision_guid is a string.\n \nThis method returns a list of revisions."
      operationId: returns-edit-revisions-identified-by-ids-in-ids-ids-can-contain-up-to-20-semicolon-delimited-ids-to-
      x-api-path-slug: revisionsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Guid list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Revisions
---