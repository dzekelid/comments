---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Create Comment
  description: Used to add a comment by the user to a specific file or comment (i.e.
    as a reply comment).
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{FILE_ID}/comments:
    get:
      summary: Get File's Comments
      description: Retrieves the comments on a particular file, if any exist.
      operationId: getFileComments
      x-api-path-slug: filesfile-idcomments-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FILE_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Comments
  /comments:
    post:
      summary: Create Comment
      description: Used to add a comment by the user to a specific file or comment
        (i.e. as a reply comment).
      operationId: createComment
      x-api-path-slug: comments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Comments
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