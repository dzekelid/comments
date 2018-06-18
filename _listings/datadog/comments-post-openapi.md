---
swagger: "2.0"
x-collection-name: Datadog
x-complete: 0
info:
  title: DataDog API Add Comments
  version: 1.0.0
  description: |-
    Comments are essentially special forms of events that
              appear in the stream. They can start a new discussion thread or
              optionally, reply in another thread.
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  comments:
    post:
      summary: Add Comments
      description: |-
        Comments are essentially special forms of events that
                  appear in the stream. They can start a new discussion thread or
                  optionally, reply in another thread.
      operationId: postComments
      x-api-path-slug: comments-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
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