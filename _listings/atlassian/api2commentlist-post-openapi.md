---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get comments by ids
  description: Returns comments for given comments ids. Only comments to which the
    user has permissions, will be included in the result. The returned set of comments
    is limited to 1000 elements.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/comment/list:
    post:
      summary: Get comments by ids
      description: Returns comments for given comments ids. Only comments to which
        the user has permissions, will be included in the result. The returned set
        of comments is limited to 1000 elements.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentListResource.getCommentsByIds_post
      x-api-path-slug: api2commentlist-post
      parameters:
      - in: query
        name: expand
        description: 'optional comma separated list of parameters to expand: renderedBody
          (provides body rendered in HTML), properties (provides comment properties)'
      responses:
        200:
          description: OK
      tags:
      - Comments
      - By
      - Ids
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