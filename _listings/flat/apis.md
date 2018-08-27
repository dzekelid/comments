---
name: Flat
x-slug: flat
description: Whether youre a beginner or a professional composer, our user-friendly
  music composition software gives you all the tools that you need to make your own
  sheet music. You can write, listen, share and discover music scores right in your
  web browser on any device
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Comments
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/apis.md
specificationVersion: "0.14"
apis:
- name: Flat - List comments
  x-api-slug: scoresscorecomments-get
  description: This method lists the different comments added on a music score (documents
    and inline) sorted by their post dates.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecomments-get-openapi.md
- name: Flat - Post a new comment
  x-api-slug: scoresscorecomments-post
  description: |-
    Post a document or a contextualized comment on a document.

    Please note that this method includes an anti-spam system for public scores. We don't guarantee that your comments will be accepted and displayed to end-user. Comments are be blocked by returning a `403` HTTP error and hidden from other users when the `spam` property is `true`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecomments-post-openapi.md
- name: Flat - Delete a comment
  x-api-slug: scoresscorecommentscomment-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscomment-delete-openapi.md
- name: Flat - Update an existing comment
  x-api-slug: scoresscorecommentscomment-put
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscomment-put-openapi.md
- name: Flat - Mark the comment as unresolved
  x-api-slug: scoresscorecommentscommentresolved-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscommentresolved-delete-openapi.md
- name: Flat - Mark the comment as resolved
  x-api-slug: scoresscorecommentscommentresolved-put
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscommentresolved-put-openapi.md
- name: Flat - Mark the comment as resolved
  x-api-slug: scoresscorecommentscommentresolved-put
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscommentresolved-put-openapi.md
- name: Flat - Mark the comment as unresolved
  x-api-slug: scoresscorecommentscommentresolved-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscommentresolved-delete-openapi.md
- name: Flat - Update an existing comment
  x-api-slug: scoresscorecommentscomment-put
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscomment-put-openapi.md
- name: Flat - Delete a comment
  x-api-slug: scoresscorecommentscomment-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecommentscomment-delete-openapi.md
- name: Flat - Post a new comment
  x-api-slug: scoresscorecomments-post
  description: |-
    Post a document or a contextualized comment on a document.

    Please note that this method includes an anti-spam system for public scores. We don't guarantee that your comments will be accepted and displayed to end-user. Comments are be blocked by returning a `403` HTTP error and hidden from other users when the `spam` property is `true`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flat-logo.png
  humanURL: http://flat.io
  baseURL: https://api.flat.io//v2
  tags: API Provider, Music, Profiles, Relative Data, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/flat/scoresscorecomments-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://fitbit.api.gallery.streamdata.io
- type: x-api-stack
  url: http://flat.stack.network
- type: x-developer
  url: https://flat.io/developers
- type: x-embeddable
  url: https://flat.io/developers/embed
- type: x-github
  url: https://github.com/FlatIO
- type: x-pricing
  url: https://flat.io/pricing
- type: x-privacy-policy
  url: https://flat.io/help/en/policies/#coppa-and-ferpa-compliance
- type: x-support
  url: https://flat.io/help
- type: x-twitter
  url: https://twitter.com/flat_io
- type: x-website
  url: http://flat.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---