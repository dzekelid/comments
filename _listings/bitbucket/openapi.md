swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 1
info:
  title: Bitbucket
  description: code-against-the-bitbucket-api-to-automate-simple-tasks-embed-bitbucket-data-into-your-own-site-build-mobile-or-desktop-apps-or-even-add-custom-ui-addons-into-bitbucket-itself-using-the-connect-framework-
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
  /repositories/{username}/{repo_slug}/commit/{sha}/comments/{comment_id}:
    get:
      summary: Get Repositories Username Repo Slug Commit Sha Comments Comment
      description: Get repositories username repo slug commit sha comments comment
      operationId: getRepositoriesUsernameRepoSlugCommitShaCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-get
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
      - Comment
    parameters:
      summary: Parameters Repositories Username Repo Slug Commit Sha Comments Comment
      description: Parameters repositories username repo slug commit sha comments
        comment
      operationId: parametersRepositoriesUsernameRepoSlugCommitShaCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters
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
      - Comment
  /repositories/{username}/{repo_slug}/issues/{issue_id}/comments:
    get:
      summary: Get Repositories Username Repo Slug Issues Issue  Comments
      description: |-
        Returns all comments that were made on the specified issue.

        The default sorting is oldest to newest and can be overridden with
        the `sort` query parameter.
      operationId: getRepositoriesUsernameRepoSlugIssuesIssueComments
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idcomments-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Comments
    parameters:
      summary: Parameters Repositories Username Repo Slug Issues Issue  Comments
      description: Parameters repositories username repo slug issues issue  comments
      operationId: parametersRepositoriesUsernameRepoSlugIssuesIssueComments
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idcomments-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Comments
  /repositories/{username}/{repo_slug}/issues/{issue_id}/comments/{comment_id}:
    get:
      summary: Get Repositories Username Repo Slug Issues Issue  Comments Comment
      description: Get repositories username repo slug issues issue  comments comment
      operationId: getRepositoriesUsernameRepoSlugIssuesIssueCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Comments
      - Comment
    parameters:
      summary: Parameters Repositories Username Repo Slug Issues Issue  Comments Comment
      description: Parameters repositories username repo slug issues issue  comments
        comment
      operationId: parametersRepositoriesUsernameRepoSlugIssuesIssueCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Comments
      - Comment
  /repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/comments:
    get:
      summary: Get Repositories Username Repo Slug Pullrequests Pull Request  Comments
      description: |-
        Returns a paginated list of the pull request's comments.

        This includes both global, inline comments and replies.

        The default sorting is oldest to newest and can be overridden with
        the `sort` query parameter.

        This endpoint also supports filtering and sorting of the results. See
        [filtering and sorting](../../../../../../meta/filtering) for more
        details.
      operationId: getRepositoriesUsernameRepoSlugPullrequestsPullRequestComments
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcomments-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Comments
    parameters:
      summary: Parameters Repositories Username Repo Slug Pullrequests Pull Request  Comments
      description: Parameters repositories username repo slug pullrequests pull request  comments
      operationId: parametersRepositoriesUsernameRepoSlugPullrequestsPullRequestComments
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcomments-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Comments
  /repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/comments/{comment_id}:
    get:
      summary: Get Repositories Username Repo Slug Pullrequests Pull Request  Comments
        Comment
      description: Get repositories username repo slug pullrequests pull request  comments
        comment
      operationId: getRepositoriesUsernameRepoSlugPullrequestsPullRequestCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Comments
      - Comment
    parameters:
      summary: Parameters Repositories Username Repo Slug Pullrequests Pull Request  Comments
        Comment
      description: Parameters repositories username repo slug pullrequests pull request  comments
        comment
      operationId: parametersRepositoriesUsernameRepoSlugPullrequestsPullRequestCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
      - ""
      - Comments
      - Comment
  /snippets/{username}/{encoded_id}/comments:
    get:
      summary: Get Snippets Username Encoded  Comments
      description: |-
        Used to retrieve a paginated list of all comments for a specific
        snippet.

        This resource works identical to commit and pull request comments.

        The default sorting is oldest to newest and can be overridden with
        the `sort` query parameter.
      operationId: getSnippetsUsernameEncodedComments
      x-api-path-slug: snippetsusernameencoded-idcomments-get
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Comments
    parameters:
      summary: Parameters Snippets Username Encoded  Comments
      description: Parameters snippets username encoded  comments
      operationId: parametersSnippetsUsernameEncodedComments
      x-api-path-slug: snippetsusernameencoded-idcomments-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Comments
    post:
      summary: Add Snippets Username Encoded  Comments
      description: |-
        Creates a new comment.

        The only required field in the body is `content.raw`.

        To create a threaded reply to an existing comment, include `parent.id`.
      operationId: postSnippetsUsernameEncodedComments
      x-api-path-slug: snippetsusernameencoded-idcomments-post
      parameters:
      - in: body
        name: _body
        description: The contents of the new comment
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Comments
  /snippets/{username}/{encoded_id}/comments/{comment_id}:
    delete:
      summary: Delete Snippets Username Encoded  Comments Comment
      description: |-
        Deletes a snippet comment.

        Comments can only be removed by their author.
      operationId: deleteSnippetsUsernameEncodedCommentsComment
      x-api-path-slug: snippetsusernameencoded-idcommentscomment-id-delete
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Comments
      - Comment
    get:
      summary: Get Snippets Username Encoded  Comments Comment
      description: Get snippets username encoded  comments comment
      operationId: getSnippetsUsernameEncodedCommentsComment
      x-api-path-slug: snippetsusernameencoded-idcommentscomment-id-get
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Comments
      - Comment
    parameters:
      summary: Parameters Snippets Username Encoded  Comments Comment
      description: Parameters snippets username encoded  comments comment
      operationId: parametersSnippetsUsernameEncodedCommentsComment
      x-api-path-slug: snippetsusernameencoded-idcommentscomment-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Comments
      - Comment
    put:
      summary: Update Snippets Username Encoded  Comments Comment
      description: |-
        Updates a comment.

        Comments can only be updated by their author.
      operationId: putSnippetsUsernameEncodedCommentsComment
      x-api-path-slug: snippetsusernameencoded-idcommentscomment-id-put
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Comments
      - Comment