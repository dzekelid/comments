---
name: GitHub
x-slug: github
description: With a community of more than 10 million people, developers can discover,
  use and contribute to over 24 million projects using a powerful, collaborative workflow.    Whether
  using GitHub.com or your own instance of GitHub Enterprise, you can integrate ...
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "70"
tags: Comments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: Github Get Gists  Comments
  x-api-slug: github
  description: List comments on a gist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////gists/{id}/comments
  tags: Gists, , Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcomments-get-openapi.md
- name: Github Add Gists  Comments
  x-api-slug: github
  description: Create a commen
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////gists/{id}/comments
  tags: Gists, , Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcomments-post-openapi.md
- name: Github Delete Gists  Comments Comment
  x-api-slug: github
  description: Delete a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////gists/{id}/comments/{commentId}
  tags: Gists, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcommentscommentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcommentscommentid-delete-openapi.md
- name: Github Get Gists  Comments Comment
  x-api-slug: github
  description: Get a single comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////gists/{id}/comments/{commentId}
  tags: Gists, , Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcommentscommentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcommentscommentid-get-openapi.md
- name: Github Patch Gists  Comments Comment
  x-api-slug: github
  description: Edit a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////gists/{id}/comments/{commentId}
  tags: Gists, , Comments, Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/gistsidcommentscommentid-patch-openapi.md
- name: Github Get Repos Owner Repo Comments
  x-api-slug: github
  description: |-
    List commit comments for a repository.
    Comments are ordered by ascending ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/comments
  tags: Repos, Owner, Repo, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocomments-get-openapi.md
- name: Github Delete Repos Owner Repo Comments Comment
  x-api-slug: github
  description: Delete a commit comment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/comments/{commentId}
  tags: Repos, Owner, Repo, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommentscommentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommentscommentid-delete-openapi.md
- name: Github Get Repos Owner Repo Comments Comment
  x-api-slug: github
  description: Get a single commit comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/comments/{commentId}
  tags: Repos, Owner, Repo, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommentscommentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommentscommentid-get-openapi.md
- name: Github Patch Repos Owner Repo Comments Comment
  x-api-slug: github
  description: Update a commit comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/comments/{commentId}
  tags: Repos, Owner, Repo, Comments, Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommentscommentid-patch-openapi.md
- name: Github Get Repos Owner Repo Commits Shacode Comments
  x-api-slug: github
  description: List comments for a single commitList comments for a single commit.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/commits/{shaCode}/comments
  tags: Repos, Owner, Repo, Commits, Shacode, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommitsshacodecomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommitsshacodecomments-get-openapi.md
- name: Github Add Repos Owner Repo Commits Shacode Comments
  x-api-slug: github
  description: Create a commit comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/commits/{shaCode}/comments
  tags: Repos, Owner, Repo, Commits, Shacode, Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepocommitsshacodecomments-post-openapi.md
- name: Github Get Repos Owner Repo Issues Comments
  x-api-slug: github
  description: List comments in a repository.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/comments
  tags: Repos, Owner, Repo, Issues, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuescomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuescomments-get-openapi.md
- name: Github Delete Repos Owner Repo Issues Comments Comment
  x-api-slug: github
  description: Delete a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/comments/{commentId}
  tags: Repos, Owner, Repo, Issues, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuescommentscommentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuescommentscommentid-delete-openapi.md
- name: Github Get Repos Owner Repo Issues Comments Comment
  x-api-slug: github
  description: Get a single comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/comments/{commentId}
  tags: Repos, Owner, Repo, Issues, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuescommentscommentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuescommentscommentid-get-openapi.md
- name: Github Patch Repos Owner Repo Issues Comments Comment
  x-api-slug: github
  description: Edit a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/comments/{commentId}
  tags: Repos, Owner, Repo, Issues, Comments, Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuescommentscommentid-patch-openapi.md
- name: Github Get Repos Owner Repo Issues Number Comments
  x-api-slug: github
  description: List comments on an issue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/{number}/comments
  tags: Repos, Owner, Repo, Issues, Number, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuesnumbercomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuesnumbercomments-get-openapi.md
- name: Github Add Repos Owner Repo Issues Number Comments
  x-api-slug: github
  description: Create a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/issues/{number}/comments
  tags: Repos, Owner, Repo, Issues, Number, Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepoissuesnumbercomments-post-openapi.md
- name: Github Get Repos Owner Repo Pulls Comments
  x-api-slug: github
  description: |-
    List comments in a repository.
    By default, Review Comments are ordered by ascending ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/pulls/comments
  tags: Repos, Owner, Repo, Pulls, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullscomments-get-openapi.md
- name: Github Delete Repos Owner Repo Pulls Comments Comment
  x-api-slug: github
  description: Delete a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/pulls/comments/{commentId}
  tags: Repos, Owner, Repo, Pulls, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullscommentscommentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullscommentscommentid-delete-openapi.md
- name: Github Get Repos Owner Repo Pulls Comments Comment
  x-api-slug: github
  description: Get a single comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/pulls/comments/{commentId}
  tags: Repos, Owner, Repo, Pulls, Comments, Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullscommentscommentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullscommentscommentid-get-openapi.md
- name: Github Patch Repos Owner Repo Pulls Comments Comment
  x-api-slug: github
  description: Edit a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/pulls/comments/{commentId}
  tags: Repos, Owner, Repo, Pulls, Comments, Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullscommentscommentid-patch-openapi.md
- name: Github Get Repos Owner Repo Pulls Number Comments
  x-api-slug: github
  description: List comments on a pull request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/pulls/{number}/comments
  tags: Repos, Owner, Repo, Pulls, Number, Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullsnumbercomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullsnumbercomments-get-openapi.md
- name: Github Add Repos Owner Repo Pulls Number Comments
  x-api-slug: github
  description: |-
    Create a comment.
      #TODO Alternative input ( http://developer.github.com/v3/pulls/comments/ )
      description: |
        Alternative Input.
        Instead of passing commit_id, path, and position you can reply to an
        existing Pull Request Comment like this:

            body
               Required string
            in_reply_to
               Required number - Comment id to reply to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/pulls/{number}/comments
  tags: Repos, Owner, Repo, Pulls, Number, Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/reposownerrepopullsnumbercomments-post-openapi.md
- name: Github
  x-api-slug: github
  description: With a community of more than 10 million people, developers can discover,
    use and contribute to over 24 million projects using a powerful, collaborative
    workflow.    Whether using GitHub.com or your own instance of GitHub Enterprise,
    you can integrate ...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/github/openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---