---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You dont have to read through a lot of discussion to find the best answer.    Like
  to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Comments
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange - Get Answer Comments
  x-api-slug: answersidscomments-get
  description: "Gets the comments on a set of answers.\n \nIf you know that you have
    an answer id and need the comments, use this method. If you know you have a question
    id, use /questions/{id}/comments. If you are unsure, use /posts/{id}/comments.\n
    \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
    look for answer_id on answer objects.\n \nThe sorts accepted by this method operate
    on the follow fields of the comment object:\n - creation - creation_date\n - votes
    - score\n  creation is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/answersidscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/answersidscomments-get-openapi.md
- name: Stack Exchange - Get Comments
  x-api-slug: comments-get
  description: "Gets all the comments on the site.\n \nIf you're filtering for interesting
    comments (by score, creation date, etc.) make use of the sort paramter with appropriate
    min and max values.\n \nIf you're looking to query conversations between users,
    instead use the /users/{ids}/mentioned and /users/{ids}/comments/{toid} methods.\n
    \nThe sorts accepted by this method operate on the follow fields of the comment
    object:\n - creation - creation_date\n - votes - score\n  creation is the default
    sort.\n \n It is possible to create moderately complex queries using sort, min,
    max, fromdate, and todate.\n \nThis method returns a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/comments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/comments-get-openapi.md
- name: Stack Exchange - Get Comment
  x-api-slug: commentsids-get
  description: "Gets the comments identified in id.\n \nThis method is most useful
    if you have a cache of comment ids obtained through other means (such as /questions/{id}/comments)
    but suspect the data may be stale.\n \n{ids} can contain up to 100 semicolon delimited
    ids, to find ids programatically look for comment_id on comment objects.\n \nThe
    sorts accepted by this method operate on the follow fields of the comment object:\n
    - creation - creation_date\n - votes - score\n  creation is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/commentsids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/commentsids-get-openapi.md
- name: Stack Exchange - Delete Comment
  x-api-slug: commentsiddelete-post
  description: "Deletes a comment.\n \nUse an access_token with write_access to delete
    a comment.\n \nIn practice, this method will never return an object."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/commentsiddelete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/commentsiddelete-post-openapi.md
- name: Stack Exchange - Edit Comment
  x-api-slug: commentsidedit-post
  description: "Edit an existing comment.\n \nUse an access_token with write_access
    to edit an existing comment.\n \nThis method return the created comment."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/commentsidedit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/commentsidedit-post-openapi.md
- name: Stack Exchange - My Comments
  x-api-slug: mecomments-get
  description: "Returns the comments owned by the user associated with the given access_token.\n
    \nThis method returns a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/mecomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/mecomments-get-openapi.md
- name: Stack Exchange - My Comments
  x-api-slug: mecommentstoid-get
  description: "Returns the comments owned by the user associated with the given access_token
    that are in reply to the user identified by {toId}.\n \nThis method returns a
    list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/mecommentstoid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/mecommentstoid-get-openapi.md
- name: Stack Exchange - Get Post Comments
  x-api-slug: postsidscomments-get
  description: "Gets the comments on the posts identified in ids, regardless of the
    type of the posts.\n \nThis method is meant for cases when you are unsure of the
    type of the post id provided. Generally, this would be due to obtaining the post
    id directly from a user.\n \n{ids} can contain up to 100 semicolon delimited ids,
    to find ids programatically look for post_id, answer_id, or question_id on post,
    answer, and question objects respectively.\n \nThe sorts accepted by this method
    operate on the follow fields of the comment object:\n - creation - creation_date\n
    - votes - score\n  creation is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/postsidscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/postsidscomments-get-openapi.md
- name: Stack Exchange - Add Comment Post
  x-api-slug: postsidcommentsadd-post
  description: "Create a new comment.\n \nUse an access_token with write_access to
    create a new comment on a post.\n \nThis method returns the created comment."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/postsidcommentsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/postsidcommentsadd-post-openapi.md
- name: Stack Exchange - Get User Comments
  x-api-slug: usersidscomments-get
  description: "Get the comments posted by users in {ids}.\n \n{ids} can contain up
    to 100 semicolon delimited ids, to find ids programatically look for user_id on
    user or shallow_user objects.\n \nThe sorts accepted by this method operate on
    the follow fields of the comment object:\n - creation - creation_date\n - votes
    - score\n  creation is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/usersidscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/usersidscomments-get-openapi.md
- name: Stack Exchange - Get User Comments Told
  x-api-slug: usersidscommentstoid-get
  description: "Get the comments that the users in {ids} have posted in reply to the
    single user identified in {toid}.\n \nThis method is useful for extracting conversations,
    especially over time or across multiple posts.\n \n{ids} can contain up to 100
    semicolon delimited ids, to find ids programatically look for user_id on user
    or shallow_user objects. {toid} can contain only 1 id, found in the same manner
    as those in {ids}.\n \nThe sorts accepted by this method operate on the follow
    fields of the comment object:\n - creation - creation_date\n - votes - score\n
    \ creation is the default sort.\n \n It is possible to create moderately complex
    queries using sort, min, max, fromdate, and todate.\n \nThis method returns a
    list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/usersidscommentstoid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/usersidscommentstoid-get-openapi.md
- name: Stack Exchange - Get Answer Comments
  x-api-slug: answersidscomments-get
  description: "Gets the comments on a set of answers.\n \nIf you know that you have
    an answer id and need the comments, use this method. If you know you have a question
    id, use /questions/{id}/comments. If you are unsure, use /posts/{id}/comments.\n
    \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
    look for answer_id on answer objects.\n \nThe sorts accepted by this method operate
    on the follow fields of the comment object:\n - creation - creation_date\n - votes
    - score\n  creation is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/answersidscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/stack-exchange/answersidscomments-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://square.api.gallery.streamdata.io
- type: x-api-stack
  url: http://stack.exchange.stack.network
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-linkedin
  url: https://www.linkedin.com/company/stack-exchange
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---