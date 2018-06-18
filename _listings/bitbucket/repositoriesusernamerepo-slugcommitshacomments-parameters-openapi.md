---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Commit Sha Comments
  description: Parameters repositories username repo slug commit sha comments
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/commit/{sha}/comments:
    get:
      summary: Get Repositories Username Repo Slug Commit Sha Comments
      description: |-
        Returns the commit's comments.

        This includes both global and inline comments.

        The default sorting is oldest to newest and can be overridden with
        the `sort` query parameter.
      operationId: getRepositoriesUsernameRepoSlugCommitShaComments
      x-api-path-slug: repositoriesusernamerepo-slugcommitshacomments-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commit
      - Sha
      - Comments
    parameters:
      summary: Parameters Repositories Username Repo Slug Commit Sha Comments
      description: Parameters repositories username repo slug commit sha comments
      operationId: parametersRepositoriesUsernameRepoSlugCommitShaComments
      x-api-path-slug: repositoriesusernamerepo-slugcommitshacomments-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commit
      - Sha
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