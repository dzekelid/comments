---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Event Comment and Reply Likes
  description: Returns lists of likes for an event comment or reply
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /comments:
    get:
      summary: Comments
      description: API method for accessing meetup group comments
      operationId: groups
      x-api-path-slug: comments-get
      parameters:
      - in: query
        name: group_id
        description: Return comments in groups with these ID numbers [separated by
          commas]
        type: string
      - in: query
        name: group_urlname
        description: Return comments for the group with this custom URL path
        type: string
      - in: query
        name: topic, groupnum
        description: Return comments for the group with given topic and number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/event_comments:
    get:
      summary: Comments v2
      description: This method returns messages that appear under Talk about this
        Meetup. To post messages, see the corresponding write method.
      operationId: events
      x-api-path-slug: 2event-comments-get
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: callback
        description: Name of a function to be called with an array of Event Comment
          notification objects
        type: string
      - in: query
        name: comment_id
        description: Return comments for a given set of comment IDs, separated by
          commas
        type: string
      - in: query
        name: event_id
        description: Limit notifications to a specific event id
        type: string
      - in: query
        name: event_id
        description: Return comments on these events, separated by commas
        type: string
      - in: query
        name: fields
        description: Optionally accepts the value member_photo or notifications
        type: string
      - in: query
        name: group_id
        description: Return comments in groups with these ID numbers, separated by
          commas
        type: string
      - in: query
        name: member_id
        description: Return comments for the given member_ids, separated by commas
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Should be supplied for all but the first polling request, so
          that any missed notifications are can be sent in an immediate response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
    ws:
      summary: WebSockets Event Comments Stream
      description: |-
        For browsers that support it, [WebSockets](http://dev.w3.org/html5/websockets/) is a more
        efficient alternative to the long-polling stream. This is a **push only** endpoint and will discard
        any messages received from the client after the socket is open.

        Because browser support for WebSockets is limited, we recommend that you consume this stream
        through the [must.js](https://github.com/meetup/must.js#readme) client, which can fallback to long-polling.
      operationId: streams
      x-api-path-slug: 2event-comments-ws
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: event_id
        description: Limit notifications to a specific event id
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Return recent Event Comments with an mtime greater than the supplied
          time, in milliseconds since the epoch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/event_comment:
    post:
      summary: Event Comment v2
      description: This method posts messages that appear under Talk about this Meetup.
      operationId: events
      x-api-path-slug: 2event-comment-post
      parameters:
      - in: query
        name: comment
        description: The comment text
        type: string
      - in: query
        name: event_id
        description: The event related to this comment
        type: string
      - in: query
        name: in_reply_to
        description: If this comment is a reply, the ID of the comment being replied
          to
        type: string
      - in: query
        name: notifications
        description: Notification control for authorized member on this comment thread
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/event_comment/:id:
    get:
      summary: Event Comment Get
      description: Retrieve a single event comment or reply
      operationId: events
      x-api-path-slug: 2event-commentid-get
      parameters:
      - in: query
        name: fields
        description: comma-separate list of optional fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
    delete:
      summary: Event Comment Delete
      description: Delete a single event comment or reply
      operationId: events
      x-api-path-slug: 2event-commentid-delete
      parameters:
      - in: query
        name: fields
        description: comma-separate list of optional fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/event_comment_flag:
    post:
      summary: Event Comment Flag
      description: This method creates a spam report for comment content
      operationId: events
      x-api-path-slug: 2event-comment-flag-post
      parameters:
      - in: query
        name: comment_id
        description: The id of the comment
        type: string
      - in: query
        name: reason
        description: Reason for flagging the comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/event_comment_subscribe/:id:
    delete:
      summary: Event Comment Unsubscribe
      description: Unsubscribe to notifications for updates to a given comment thread
      operationId: events
      x-api-path-slug: 2event-comment-subscribeid-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/event_comment_like/:id:
    post:
      summary: Event Comment Like
      description: Like a given Event comment
      operationId: events
      x-api-path-slug: 2event-comment-likeid-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
    delete:
      summary: Event Comment Unlike
      description: Unlike a given Event comment
      operationId: events
      x-api-path-slug: 2event-comment-likeid-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/event_comment_likes:
    get:
      summary: Comment Likes
      description: Api for listing likes of a given event comment
      operationId: events
      x-api-path-slug: 2event-comment-likes-get
      parameters:
      - in: query
        name: comment_id
        description: Return likes for a given comment_id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /2/photo_comment:
    post:
      summary: Photo Comment v2
      description: This method posts comments that appear below photos
      operationId: photos
      x-api-path-slug: 2photo-comment-post
      parameters:
      - in: query
        name: comment
        description: The comment text
        type: string
      - in: query
        name: photo_id
        description: The photo related to this comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
  /2/photo_albums:
    get:
      summary: Photo Albums
      description: This method returns photo albums associated with Meetup groups.
        To create albums, see the corresponding write method.
      operationId: photos
      x-api-path-slug: 2photo-albums-get
      parameters:
      - in: query
        name: event_id
        description: Return photo albums for these event ids, separated by commas
        type: string
      - in: query
        name: group_id
        description: Return albums in groups with these ID, separated by commas
        type: string
      - in: query
        name: photo_album_id
        description: Return albums with these IDs, separated by commas
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
  /:urlname/events/:event_id/comments:
    get:
      summary: Event Comments List
      description: |-
        Lists the comments and replies posted in a given Meetup Event.

        To view the list of likes for a comment or reply
        see the [likes](/meetup_api/docs/:urlname/events/:event_id/comments/:comment_id/likes/)
        endpoint
      operationId: comments
      x-api-path-slug: urlnameeventsevent-idcomments-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
    post:
      summary: Event comment and reply
      description: Creates new comments and replies to existing comments within an
        Meetup event
      operationId: comments
      x-api-path-slug: urlnameeventsevent-idcomments-post
      parameters:
      - in: query
        name: comment
        description: The text of the comment in at most 1024 characters
        type: string
      - in: query
        name: in_reply_to
        description: If posting a reply, set this to the numeric identifier of the
          associated top level comment
        type: string
      - in: query
        name: notifications
        description: A boolean value indicating whether or not you wish to recieve
          future notifications about updates to this comment thread
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /:urlname/events/:event_id/comments/:comment_id:
    delete:
      summary: Event comment delete
      description: Deletes comments posted in events
      operationId: comments
      x-api-path-slug: urlnameeventsevent-idcommentscomment-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /:urlname/events/:event_id/comments/:comment_id/likes:
    get:
      summary: Event Comment and Reply Likes
      description: Returns lists of likes for an event comment or reply
      operationId: comments
      x-api-path-slug: urlnameeventsevent-idcommentscomment-idlikes-get
      responses:
        200:
          description: OK
      tags:
      - Events
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