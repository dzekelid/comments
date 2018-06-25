---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Comments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework Delete a comment
  x-api-slug: open-science-framework
  description: |-
    Deletes a comment. This action can be undone by setting deleted to False in a comment update request.
    #### Returns
    If the request is successful, no content is returned.

    If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//comments/{comment_id}/
  tags: Comments,Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-openapi.md
- name: Open Science Framework Retrieve a comment
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a comment
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested comment, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//comments/{comment_id}/
  tags: Comments,Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-openapi.md
- name: Open Science Framework Update a comment
  x-api-slug: open-science-framework
  description: |-
    Updates the specified comment by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
    #### Returns
    Returns JSON with a `data` key containing the new representation of the updated comment, if the request is successful.

    If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//comments/{comment_id}/
  tags: Comments,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-put-openapi.md
- name: Open Science Framework List all comments
  x-api-slug: open-science-framework
  description: |-
    A paginated list of comments related to a given node.

    The returned comments are sorted by their creation date, with the most recent comments appearing first.
    ####Permissions
    Comments on public nodes are given read-only access to everyone.

    If the node comment-level is `private`, only contributors have permission to comment.

    If the comment-level is `public`, any logged-in OSF user can comment.

    Comments on private nodes are only visible to contributors and administrators on the parent node.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of comment objects. Each resource in the array is a separate comment object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include comments that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/comments/?filter[target_id]=jg7sezmdnt93

    Nodes may be filtered by their `deleted`, `target_id`, `date_created`, `date_modified`.

    Most fields are string fields and will be filtered using simple substring matching. Public and preprint are boolean fields, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting `true` or `false` in the query will cause the match to fail.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/comments/
  tags: Nodes,Node,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/nodesnode-idcomments-get-openapi.md
- name: Open Science Framework Create a comment
  x-api-slug: open-science-framework
  description: |-
    Create a comment on a given node overview page or a reply to a comment on that node.

    To create a comment on the node overview page, the target `type` would be "nodes" and the target `id` would be the node `id`.

    To reply to a comment on this node, the target `type` would be "comments" and the target `id` would be the `id` of the comment to reply to.
    ####Required
    A relationship object with a `data` key, containing the target (`comments` or `nodes`) type and a target `id` is required.
    In addition, the `content` attribute describing the relationship between the node and the comment is required.
    ####Returns
    Returns a JSON object with a data key containing the representation of the new comment, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/comments/
  tags: Nodes,Node,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/nodesnode-idcomments-post-openapi.md
- name: Open Science Framework List all comments
  x-api-slug: open-science-framework
  description: |-
    A paginated list of the registration's comments.

    The returned comments are sorted by their creation date, with the most recent comments appearing first.
    ####Permissions
    Comments of public registrations are given read-only access to everyone.

    If the comment-level is `private`, only registration contributors have permission to comment.

    If the comment-level is `public`, any logged-in OSF user can comment.

    Comments of private registrations are only visible to contributors and administrators on the registration.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of comment objects. Each resource in the array is a separate comment object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include comments that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wuerf/comments/?filter[target]=wuerf

    Comments may be filtered by their `deleted`, `target`, `date_created`, `date_modified`.

    Most fields are string fields and will be filtered using simple substring matching. Deleted is a boolean field, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting `true` or `false` in the query will cause the match to fail.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/comments/
  tags: Registrations,Registration,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/registrationsregistration-idcomments-get-openapi.md
- name: Open Science Framework
  x-api-slug: open-science-framework
  description: OSF provides free and open source project management support for researchers
    across the entire research lifecycle. As a collaboration tool, OSF helps researchers
    work on projects privately with a limited number of collaborators and make parts
    of their projects public, or make all the project publicly accessible for broader
    dissemination. As a workflow system, OSF enables connections to the many services
    researchers already use to streamline their process and increase efficiency. As
    a flexible repository, it can store and archive research data, protocols, and
    materials.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---