swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Plivo
  version: 1.0.0
host: api.plivo.com
basePath: v1/
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
  /photos/:id/comments:
    post:
      summary: Post Photos Comments
      description: Creates a new comment for the photo.
      operationId: creates-a-new-comment-for-the-photo
      x-api-path-slug: photosidcomments-post
      parameters:
      - in: query
        name: body (required)
        description: Content of the comment
      - in: query
        name: id (required)
        description: The Photo ID to post comments for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
      - Comments