---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List feedback comments
  description: Lists feedback comments.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/comments/{referenceType}/{referenceValue}:
    get:
      summary: List comments
      description: Lists comments. The reference type and the reference value must
        be specified (e.g. the reference type is 'order' and the reference value is
        the ID of the order).
      operationId: getRestCommentsReferencetypeReferencevalue
      x-api-path-slug: restcommentsreferencetypereferencevalue-get
      parameters:
      - in: query
        name: isVisibleForContact
        description: If true, the comment is visible for the associated contact
      - in: path
        name: referenceType
      - in: path
        name: referenceValue
      - in: query
        name: userId
        description: The ID of the user the comment belongs to
      responses:
        200:
          description: OK
      tags:
      - List
      - Comments
  /rest/feedbacks/comments:
    get:
      summary: List feedback comments
      description: Lists feedback comments.
      operationId: getRestFeedbacksComments
      x-api-path-slug: restfeedbackscomments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
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