---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Photosets Comments Edit Comment
  description: Edit the text of a comment as the currently authenticated user.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.photos.comments.addComment:
    post:
      summary: Photos Comments Add Comment
      description: Add comment to a photo as the currently authenticated user.
      operationId: postRestMethodFlickr.photos.comments.addcomment
      x-api-path-slug: restmethodflickr-photos-comments-addcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_text
        description: Text of the comment
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to add a comment to
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - AddComment
  /rest/?method=flickr.photos.comments.deleteComment:
    post:
      summary: Photos Comments Delete Comment
      description: Delete comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photos.comments.deletecomment
      x-api-path-slug: restmethodflickr-photos-comments-deletecomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to delete a comment from
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - DeleteComment
  /rest/?method=flickr.photos.comments.editComment:
    post:
      summary: Photos Comments Edit Comment
      description: Edit the text of a comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photos.comments.editcomment
      x-api-path-slug: restmethodflickr-photos-comments-editcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_id
        description: The id of the comment to edit
      - in: query
        name: comment_text
        description: Update the comment to this text
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - EditComment
  /rest/?method=flickr.photos.comments.getList:
    get:
      summary: Photos Comments Get List
      description: Returns the comments for a photo.
      operationId: getRestMethodFlickr.photos.comments.getlist
      x-api-path-slug: restmethodflickr-photos-comments-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: max_comment_date
        description: Maximum date that a comment was added
      - in: query
        name: min_comment_date
        description: Minimum date that a comment was added
      - in: query
        name: photo_id
        description: The id of the photo to fetch comments for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - GetList
  /rest/?method=flickr.photos.comments.getRecentForContacts:
    get:
      summary: Photos Comments Get Recent For Contacts
      description: Return the list of photos belonging to your contacts that have
        been commented on recently.
      operationId: getRestMethodFlickr.photos.comments.getrecentforcontacts
      x-api-path-slug: restmethodflickr-photos-comments-getrecentforcontacts-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: contacts_filter
        description: A comma-separated list of contact NSIDs to limit the scope of
          the query to
      - in: query
        name: date_lastcomment
        description: Limits the resultset to photos that have been commented on since
          this date
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - GetRecentForContacts
  /rest/?method=flickr.photosets.comments.addComment:
    post:
      summary: Photosets Comments Add Comment
      description: Add a comment to a photoset.
      operationId: postRestMethodFlickr.photosets.comments.addcomment
      x-api-path-slug: restmethodflickr-photosets-comments-addcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_text
        description: Text of the comment
      - in: query
        name: format
        description: Response format
      - in: query
        name: photoset_id
        description: The id of the photoset to add a comment to
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Comments
      - AddComment
  /rest/?method=flickr.photosets.comments.deleteComment:
    post:
      summary: Photosets Comments Delete Comment
      description: Delete a photoset comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photosets.comments.deletecomment
      x-api-path-slug: restmethodflickr-photosets-comments-deletecomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_id
        description: The id of the comment to delete from a photoset
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Comments
      - DeleteComment
  /rest/?method=flickr.photosets.comments.editComment:
    post:
      summary: Photosets Comments Edit Comment
      description: Edit the text of a comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photosets.comments.editcomment
      x-api-path-slug: restmethodflickr-photosets-comments-editcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_id
        description: The id of the comment to edit
      - in: query
        name: comment_text
        description: Update the comment to this text
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Comments
      - EditComment
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