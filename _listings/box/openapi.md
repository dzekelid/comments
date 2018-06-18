---
swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  description: the-box-content-api-gives-you-access-to-secure-content-management-and-content-experience-features-for-use-in-your-own-app--it-strives-to-be-restful-and-is-organized-around-the-main-resources-youre-familiar-with-from-the-box-web-interface-
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
---