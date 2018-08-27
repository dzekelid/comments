---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Comment Likes
  description: All the likes on this comment
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{album}/comments:
    get:
      summary: Get Album Comments
      description: The comments made on this album
      operationId: getAlbumComments
      x-api-path-slug: albumcomments-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Comments
    post:
      summary: Post Album Comments
      description: Posts a comment on the album
      operationId: postAlbumComments
      x-api-path-slug: albumcomments-post
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Album
      - Comments
  /{checkin}/comments:
    get:
      summary: Get Checkin Comments
      description: All of the comments on this checkin.
      operationId: getCheckinComments
      x-api-path-slug: checkincomments-get
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Comments
    post:
      summary: Post Checkin Comments
      description: Posts a comment to this checkin.
      operationId: postCheckinComments
      x-api-path-slug: checkincomments-post
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Comments
  /{link}/comments:
    get:
      summary: Get Link Comments
      description: All of the comments on this link.
      operationId: getLinkComments
      x-api-path-slug: linkcomments-get
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      responses:
        200:
          description: OK
      tags:
      - Link
      - Comments
    post:
      summary: Post Link Comments
      description: Posts a comment to this link.
      operationId: postLinkComments
      x-api-path-slug: linkcomments-post
      parameters:
      - in: path
        name: link
        description: Represents the ID of the link object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Link
      - Comments
  /{note}/comments:
    get:
      summary: Get Note Comments
      description: All of the comments on this note.
      operationId: getNoteComments
      x-api-path-slug: notecomments-get
      parameters:
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
      - Comments
    post:
      summary: Post Note Comments
      description: Posts a comment to this note.
      operationId: postNoteComments
      x-api-path-slug: notecomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: note
        description: Represents the ID of the note object
      responses:
        200:
          description: OK
      tags:
      - Note
      - Comments
  /{photo}/comments:
    get:
      summary: Get Photo Comments
      description: All of the comments on this photo.
      operationId: getPhotoComments
      x-api-path-slug: photocomments-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Comments
    post:
      summary: Post Photo Comments
      description: Posts a comment to this photo.
      operationId: postPhotoComments
      x-api-path-slug: photocomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
      - Comments
  /{post}/comments:
    get:
      summary: Get Add Comments
      description: All of the comments on this post.
      operationId: getAddComments
      x-api-path-slug: postcomments-get
      parameters:
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
      - Comments
    post:
      summary: Post Add Comments
      description: Posts a comment to this post.
      operationId: postAddComments
      x-api-path-slug: postcomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: post
        description: Represents the ID of the post object
      responses:
        200:
          description: OK
      tags:
      - Post
      - Comments
  /{status}/comments:
    get:
      summary: Get Status Comments
      description: All of the comments on this status.
      operationId: getStatusComments
      x-api-path-slug: statuscomments-get
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Comments
    post:
      summary: Post Status Comments
      description: Posts a comment to this status.
      operationId: postStatusComments
      x-api-path-slug: statuscomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Comments
  /{video}/comments:
    get:
      summary: Get Veo Comments
      description: All of the comments on this video.
      operationId: getVeoComments
      x-api-path-slug: videocomments-get
      parameters:
      - in: path
        name: video
        description: Represents the ID of the video object
      responses:
        200:
          description: OK
      tags:
      - Video
      - Comments
    post:
      summary: Post Veo Comments
      description: Posts a comment to this video.
      operationId: postVeoComments
      x-api-path-slug: videocomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: video
        description: Represents the ID of the video object
      responses:
        200:
          description: OK
      tags:
      - Video
      - Comments
  /{comment}:
    get:
      summary: Get Comment
      description: Returns a comment
      operationId: getComment
      x-api-path-slug: comment-get
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
    delete:
      summary: Delete Comment
      description: Deletes a comment
      operationId: deleteComment
      x-api-path-slug: comment-delete
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
  /{comment}/likes:
    get:
      summary: Get Comment Likes
      description: All the likes on this comment
      operationId: getCommentLikes
      x-api-path-slug: commentlikes-get
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Likes
    post:
      summary: Post Comment Likes
      description: Likes the comment
      operationId: postCommentLikes
      x-api-path-slug: commentlikes-post
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Likes
    delete:
      summary: Delete Comment Likes
      description: Unlikes the comment
      operationId: deleteCommentLikes
      x-api-path-slug: commentlikes-delete
      parameters:
      - in: path
        name: comment
        description: Represents the ID of the comment object
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Likes
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