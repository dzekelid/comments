---
swagger: "2.0"
x-collection-name: Blogger
x-complete: 1
info:
  title: Blogger
  description: api-for-access-to-the-data-within-blogger-
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
    get:
      summary: Get Blog Post Comment
      description: Gets one comment by ID.
      operationId: blogger.comments.get
      x-api-path-slug: blogsblogidpostspostidcommentscommentid-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to containing the comment
      - in: path
        name: commentId
        description: The ID of the comment to get
      - in: path
        name: postId
        description: ID of the post to fetch posts from
      - in: query
        name: view
        description: 'Access level for the requested comment (default: READER)'
      responses:
        200:
          description: OK
      tags:
      - Comments
  /blogs/{blogId}/posts/{postId}/comments/{commentId}/approve:
    post:
      summary: Update Blog Post Comment
      description: Marks a comment as not spam.
      operationId: blogger.comments.approve
      x-api-path-slug: blogsblogidpostspostidcommentscommentidapprove-post
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: path
        name: commentId
        description: The ID of the comment to mark as not spam
      - in: path
        name: postId
        description: The ID of the Post
      responses:
        200:
          description: OK
      tags:
      - Comments
  /blogs/{blogId}/posts/{postId}/comments/{commentId}/removecontent:
    post:
      summary: Update Blog Post Comment
      description: Removes the content of a comment.
      operationId: blogger.comments.removeContent
      x-api-path-slug: blogsblogidpostspostidcommentscommentidremovecontent-post
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: path
        name: commentId
        description: The ID of the comment to delete content from
      - in: path
        name: postId
        description: The ID of the Post
      responses:
        200:
          description: OK
      tags:
      - Comments
  /blogs/{blogId}/posts/{postId}/comments/{commentId}/spam:
    post:
      summary: Update Blog Post Comment SPAM
      description: Marks a comment as spam.
      operationId: blogger.comments.markAsSpam
      x-api-path-slug: blogsblogidpostspostidcommentscommentidspam-post
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: path
        name: commentId
        description: The ID of the comment to mark as spam
      - in: path
        name: postId
        description: The ID of the Post
      responses:
        200:
          description: OK
      tags:
      - Comments
---