---
swagger: "2.0"
info:
  title: Meetup Event Comments List
  description: |-
    Lists the comments and replies posted in a given Meetup Event.

    To view the list of likes for a comment or reply
    see the [likes](/meetup_api/docs/:urlname/events/:event_id/comments/:comment_id/likes/)
    endpoint
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
  /:urlname/events/:event_id/comments:
    get:
      summary: Event Comments List
      description: Lists the comments and replies posted in a given Meetup Event
      operationId: comments
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - comments
definitions: []
x-collection-name: Meetup
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