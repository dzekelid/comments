---
swagger: "2.0"
x-collection-name: Google Plus
x-complete: 1
info:
  title: Google Plus
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities/{activityId}/comments:
    get:
      summary: Get Activity Comments
      description: List all of the comments for an activity.
      operationId: plus.comments.list
      x-api-path-slug: activitiesactivityidcomments-get
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get comments for
      - in: query
        name: maxResults
        description: The maximum number of comments to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: sortOrder
        description: The order in which to sort the list of comments
      responses:
        200:
          description: OK
      tags:
      - Comment
---