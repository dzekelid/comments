---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Comments Comments
  description: Creates a reply to an existing comment. Comments can only be nested
    one level deep, you cannot reply to a reply of a comment. If a comment has a non-null
    parent_id value then it cannot be replied to.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blogs/:id/comments:
    post:
      summary: Post Blogs Comments
      description: Creates a comment for the Story.
      operationId: creates-a-comment-for-the-story
      x-api-path-slug: blogsidcomments-post
      parameters:
      - in: query
        name: body (required)
        description: Content of the comment
      - in: query
        name: id (required)
        description: The Story ID to create a comment for
      responses:
        200:
          description: OK
      tags:
      - Blogs
      - :id
      - Comments
  /comments/:id/comments:
    post:
      summary: Post Comments Comments
      description: Creates a reply to an existing comment. Comments can only be nested
        one level deep, you cannot reply to a reply of a comment. If a comment has
        a non-null parent_id value then it cannot be replied to.
      operationId: creates-a-reply-to-an-existing-comment-comments-can-only-be-nested-one-level-deep-you-cannot-reply-t
      x-api-path-slug: commentsidcomments-post
      parameters:
      - in: query
        name: body (required)
        description: Content of the comment
      responses:
        200:
          description: OK
      tags:
      - Comments
      - :id
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