---
swagger: "2.0"
x-collection-name: Blogger
x-complete: 0
info:
  title: Blogger API Delete Blog Post Comments
  description: Delete a comment by ID.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /blogger/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blogs/{blogId}/posts/{postId}/comments:
    get:
      summary: Get Blog Post Comments
      description: Retrieves the comments for a post, possibly filtered.
      operationId: blogger.comments.list
      x-api-path-slug: blogsblogidpostspostidcomments-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch comments from
      - in: query
        name: endDate
        description: Latest date of comment to fetch, a date-time with RFC 3339 formatting
      - in: query
        name: fetchBodies
        description: Whether the body content of the comments is included
      - in: query
        name: maxResults
        description: Maximum number of comments to include in the result
      - in: query
        name: pageToken
        description: Continuation token if request is paged
      - in: path
        name: postId
        description: ID of the post to fetch posts from
      - in: query
        name: startDate
        description: Earliest date of comment to fetch, a date-time with RFC 3339
          formatting
      - in: query
        name: status
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
      - Comments
  /blogs/{blogId}/posts/{postId}/comments/{commentId}:
    delete:
      summary: Delete Blog Post Comments
      description: Delete a comment by ID.
      operationId: blogger.comments.delete
      x-api-path-slug: blogsblogidpostspostidcommentscommentid-delete
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: path
        name: commentId
        description: The ID of the comment to delete
      - in: path
        name: postId
        description: The ID of the Post
      responses:
        200:
          description: OK
      tags:
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