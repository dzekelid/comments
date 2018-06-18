---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Comments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: bitbucket
  description: |-
    Returns the commit's comments.

    This includes both global and inline comments.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{sha}/comments
  tags: Repositories, Username, Repo, Slug, Commit, Sha, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug commit sha comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{sha}/comments
  tags: Repositories, Username, Repo, Slug, Commit, Sha, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Commit Sha Comments Comment
  x-api-slug: bitbucket
  description: Get repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{sha}/comments/{comment_id}
  tags: Repositories, Username, Repo, Slug, Commit, Sha, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Commit Sha Comments Comment
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{sha}/comments/{comment_id}
  tags: Repositories, Username, Repo, Slug, Commit, Sha, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Issues Issue  Comments
  x-api-slug: bitbucket
  description: |-
    Returns all comments that were made on the specified issue.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/comments
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Issues Issue  Comments
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug issues issue  comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/comments
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-parameters-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Issues Issue  Comments Comment
  x-api-slug: bitbucket
  description: Get repositories username repo slug issues issue  comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/comments/{comment_id}
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Issues Issue  Comments
    Comment
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug issues issue  comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/issues/{issue_id}/comments/{comment_id}
  tags: Repositories, Username, Repo, Slug, Issues, Issue, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-parameters-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Pullrequests Pull Request  Comments
  x-api-slug: bitbucket
  description: |-
    Returns a paginated list of the pull request's comments.

    This includes both global, inline comments and replies.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.

    This endpoint also supports filtering and sorting of the results. See
    [filtering and sorting](../../../../../../meta/filtering) for more
    details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/comments
  tags: Repositories, Username, Repo, Slug, Pullrequests, Pull, Request, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Pullrequests Pull Request  Comments
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug pullrequests pull request  comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/comments
  tags: Repositories, Username, Repo, Slug, Pullrequests, Pull, Request, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-parameters-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Pullrequests Pull Request  Comments
    Comment
  x-api-slug: bitbucket
  description: Get repositories username repo slug pullrequests pull request  comments
    comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/comments/{comment_id}
  tags: Repositories, Username, Repo, Slug, Pullrequests, Pull, Request, , Comments,
    Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Pullrequests Pull Request  Comments
    Comment
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug pullrequests pull request  comments
    comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/comments/{comment_id}
  tags: Repositories, Username, Repo, Slug, Pullrequests, Pull, Request, , Comments,
    Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-parameters-openapi.md
- name: Bitbucket Get Snippets Username Encoded  Comments
  x-api-slug: bitbucket
  description: |-
    Used to retrieve a paginated list of all comments for a specific
    snippet.

    This resource works identical to commit and pull request comments.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//snippets/{username}/{encoded_id}/comments
  tags: Snippets, Username, Encoded, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcomments-get-openapi.md
- name: Bitbucket Parameters Snippets Username Encoded  Comments
  x-api-slug: bitbucket
  description: Parameters snippets username encoded  comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//snippets/{username}/{encoded_id}/comments
  tags: Snippets, Username, Encoded, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcomments-parameters-openapi.md
- name: Bitbucket Add Snippets Username Encoded  Comments
  x-api-slug: bitbucket
  description: |-
    Creates a new comment.

    The only required field in the body is `content.raw`.

    To create a threaded reply to an existing comment, include `parent.id`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//snippets/{username}/{encoded_id}/comments
  tags: Snippets, Username, Encoded, , Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcomments-post-openapi.md
- name: Bitbucket Delete Snippets Username Encoded  Comments Comment
  x-api-slug: bitbucket
  description: |-
    Deletes a snippet comment.

    Comments can only be removed by their author.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//snippets/{username}/{encoded_id}/comments/{comment_id}
  tags: Snippets, Username, Encoded, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-delete-openapi.md
- name: Bitbucket Get Snippets Username Encoded  Comments Comment
  x-api-slug: bitbucket
  description: Get snippets username encoded  comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//snippets/{username}/{encoded_id}/comments/{comment_id}
  tags: Snippets, Username, Encoded, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-get-openapi.md
- name: Bitbucket Parameters Snippets Username Encoded  Comments Comment
  x-api-slug: bitbucket
  description: Parameters snippets username encoded  comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//snippets/{username}/{encoded_id}/comments/{comment_id}
  tags: Snippets, Username, Encoded, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-parameters-openapi.md
- name: Bitbucket Update Snippets Username Encoded  Comments Comment
  x-api-slug: bitbucket
  description: |-
    Updates a comment.

    Comments can only be updated by their author.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//snippets/{username}/{encoded_id}/comments/{comment_id}
  tags: Snippets, Username, Encoded, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/snippetsusernameencoded-idcommentscomment-id-put-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---