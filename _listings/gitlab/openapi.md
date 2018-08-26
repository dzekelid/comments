---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/repository/commits/{sha}/comments:
    get:
      summary: Get Projects Repository Commits Sha Comments
      description: Get projects repository commits sha comments.
      operationId: getV3ProjectsIdRepositoryCommitsShaComments
      x-api-path-slug: v3projectsidrepositorycommitsshacomments-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: path
        name: sha
        description: A commit sha, or the name of a branch or tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Comments
    post:
      summary: Post Projects Repository Commits Sha Comments
      description: Post projects repository commits sha comments.
      operationId: postV3ProjectsIdRepositoryCommitsShaComments
      x-api-path-slug: v3projectsidrepositorycommitsshacomments-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: line
        description: The line number
      - in: formData
        name: line_type
        description: The type of the line
      - in: formData
        name: note
        description: The text of the comment
      - in: formData
        name: path
        description: The file path
      - in: path
        name: sha
        description: The commits SHA
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Comments
  /v3/projects/{id}/merge_request/{merge_request_id}/comments:
    get:
      summary: Get Projects Merge Request Merge Request Comments
      description: Get projects merge request merge request comments.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcomments-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Comments
    post:
      summary: Post Projects Merge Request Merge Request Comments
      description: Post projects merge request merge request comments.
      operationId: postV3ProjectsIdMergeRequestMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcomments-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: formData
        name: note
        description: The text of the comment
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Comments
  /v3/projects/{id}/merge_requests/{merge_request_id}/comments:
    get:
      summary: Get Projects Merge Requests Merge Request Comments
      description: Get projects merge requests merge request comments.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcomments-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Comments
    post:
      summary: Post Projects Merge Requests Merge Request Comments
      description: Post projects merge requests merge request comments.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcomments-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: formData
        name: note
        description: The text of the comment
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Comments
---