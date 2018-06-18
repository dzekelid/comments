---
name: UK National Archives Discovery
x-slug: uk-national-archives-discovery
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Comments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/uk-national-archives-discovery/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Search API Get Boards Board Comments
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> get comments from a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Boards,Board,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/uk-national-archives-discovery/v3boardsboard-idcomments-get-openapi.md
- name: Getty Images Search API Post Boards Board Comments
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> add a comment to a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Boards,Board,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/uk-national-archives-discovery/v3boardsboard-idcomments-post-openapi.md
- name: Getty Images Search API Delete Boards Board Comments Comment
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> delete a comment from a board.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments/{comment_id}
  tags: Boards,Board,Comments,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/uk-national-archives-discovery/v3boardsboard-idcommentscomment-id-delete-openapi.md
- name: Getty Images Search API
  x-api-slug: getty-images-search-api
  description: Our set of APIs enable seamless integration of Getty Images expansive
    content, powerful search and rich metadata directly into your internal workflows,
    products and services. With Connects API solutions, you can fully control, customize
    and scale as you grow.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com//
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/uk-national-archives-discovery/openapi.md
x-common:
- type: x-website
  url: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
- type: x-website
  url: http:///Search
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---