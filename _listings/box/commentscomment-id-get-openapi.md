---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get Comment
  description: Used to retrieve the message and metadata about a specific comment.
    Information about the user who created the comment is also included.
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
  /comments/{COMMENT_ID}:
    get:
      summary: Get Comment
      description: Used to retrieve the message and metadata about a specific comment.
        Information about the user who created the comment is also included.
      operationId: getComment
      x-api-path-slug: commentscomment-id-get
      parameters:
      - in: path
        name: COMMENT_ID
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Comments
      - Comment
    put:
      summary: Update Comment
      description: Used to update the message of the comment.
      operationId: updateComment
      x-api-path-slug: commentscomment-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: COMMENT_ID
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Comments
      - Comment
    delete:
      summary: Delete Comment
      description: Permanently deletes a comment.
      operationId: deleteComment
      x-api-path-slug: commentscomment-id-delete
      parameters:
      - in: path
        name: COMMENT_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Comments
      - Comment
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