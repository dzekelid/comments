---
swagger: "2.0"
x-collection-name: 500px
x-complete: 0
info:
  title: 500px Get Blogs Comments
  description: Returns a listing of twenty comments for a specific Story.
  version: v1
host: api.500px.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blogs/:id/comments:
    get:
      summary: Get Blogs Comments
      description: Returns a listing of twenty comments for a specific Story.
      operationId: getBlogsComments
      x-api-path-slug: blogsidcomments-get
      parameters:
      - in: query
        name: id (required)
        description: The Story ID to get comments for
      - in: query
        name: page
        description: Return a specific page in the comment listing
      responses:
        200:
          description: OK
      tags:
      - Blogs
      - Comments
    post:
      summary: Post Blogs Comments
      description: Creates a comment for the Story.
      operationId: postBlogsComments
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
      - Comments
  /comments/:id/comments:
    post:
      summary: Post Comments Comments
      description: Creates a reply to an existing comment. Comments can only be nested
        one level deep, you cannot reply to a reply of a comment. If a comment has
        a non-null parent_id value then it cannot be replied to.
      operationId: postCommentsComments
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
      - Comments
  /photos/:id/comments:
    get:
      summary: Get Photos Comments
      description: Returns a listing of twenty comments for the photo.
      operationId: getPhotosComments
      x-api-path-slug: photosidcomments-get
      parameters:
      - in: query
        name: id (required)
        description: The Photo ID to get comments for
      - in: query
        name: nested - Include this parameter to return the comments in nested format.
      - in: query
        name: page
        description: Return a specific page in the comment listing
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
    post:
      summary: Post Photos Comments
      description: Creates a new comment for the photo.
      operationId: postPhotosComments
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
      - Comments
  /photos/{id}/comments:
    get:
      summary: Get Photos Comments
      description: Returns a listing of twenty comments for the photo.
      operationId: getPhotosComments
      x-api-path-slug: photosidcomments-get
      parameters:
      - in: path
        name: id
        description: The Photo ID
      - in: query
        name: page
        description: Return a specific page in the comment listing
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
    post:
      summary: Post Photos Comments
      description: Creates a new comment for the photo.
      operationId: postPhotosComments
      x-api-path-slug: photosidcomments-post
      parameters:
      - in: query
        name: body
        description: Content of the comment
      - in: path
        name: id
        description: The Photo ID to post comments for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
  /blogs/{id}/comments:
    get:
      summary: Get Blogs Comments
      description: Returns a listing of twenty comments for a specific Story.
      operationId: getBlogsComments
      x-api-path-slug: blogsidcomments-get
      parameters:
      - in: path
        name: id
        description: The Story ID to get comments for
      - in: query
        name: page
        description: Return a specific page in the comment listing
      responses:
        200:
          description: OK
      tags:
      - Blogs
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