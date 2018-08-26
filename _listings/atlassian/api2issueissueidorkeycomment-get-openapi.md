---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get comments
  description: |-
    Returns all comments for an issue.

    Results can be ordered by the "created" field which means the date a comment was added.
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
  /api/2/issue/{issueIdOrKey}/comment:
    get:
      summary: Get comments
      description: |-
        Returns all comments for an issue.

        Results can be ordered by the "created" field which means the date a comment was added.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentResource.getComments_get
      x-api-path-slug: api2issueissueidorkeycomment-get
      parameters:
      - in: query
        name: expand
        description: 'optional flags: renderedBody (provides body rendered in HTML)'
      - in: path
        name: issueIdOrKey
        description: to get comments for
      - in: query
        name: maxResults
        description: how many results on the page should be included
      - in: query
        name: orderBy
        description: ordering of the results
      - in: query
        name: startAt
        description: the page offset, if not specified then defaults to 0
      responses:
        200:
          description: OK
      tags:
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