---
swagger: "2.0"
x-collection-name: Datadog
x-complete: 1
info:
  title: DataDog Merged API
  version: 1.0.0
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  comments:
    post:
      summary: Add Comments
      description: |-
        Comments are essentially special forms of events that
                  appear in the stream. They can start a new discussion thread or
                  optionally, reply in another thread.
      operationId: postComments
      x-api-path-slug: comments-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
  comments/:comment_id:
    put:
      summary: Put Comments Comment
      description: PUT comments comment
      operationId: putCommentsComment
      x-api-path-slug: commentscomment-id-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
      - Comment
    delete:
      summary: Delete Comments Comment
      description: DELETE comments comment
      operationId: deleteCommentsComment
      x-api-path-slug: commentscomment-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
      - Comment
---