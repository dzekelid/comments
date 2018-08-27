---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API Update Hosted Zone Comment
  version: 1.0.0
  description: Updates the hosted zone comment. Send a POST request to the/2013-04-01/hostedzone/hosted
    zone ID             resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone/Id:
    post:
      summary: Update Hosted Zone Comment
      description: Updates the hosted zone comment. Send a POST request to the/2013-04-01/hostedzone/hosted
        zone ID             resource.
      operationId: updatehostedzonecomment
      x-api-path-slug: 20130401hostedzoneid-post
      parameters:
      - in: body
        name: Comment
        description: The new comment for the hosted zone
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: The ID for the hosted zone for which you want to update the comment
        type: string
      - in: body
        name: UpdateHostedZoneCommentRequest
        description: Root level tag for the UpdateHostedZoneCommentRequest parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hosted Zones
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