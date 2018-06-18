---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Event Comment v2
  description: This method posts messages that appear under Talk about this Meetup.
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