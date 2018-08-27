swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{projectId}/activities/{activityId}/comments:
    get:
      summary: Get a list of comments belonging to this activity.
      description: Get a list of comments belonging to this activity..
      operationId: getActivityComments
      x-api-path-slug: projectsprojectidactivitiesactivityidcomments-get
      parameters:
      - in: path
        name: activityId
        description: Activity ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
      - ActivityId
      - Comments
  /projects/{projectId}/comments:
    get:
      summary: Get a list of activity comments throughout the whole project.
      description: Get a list of activity comments throughout the whole project..
      operationId: getComments
      x-api-path-slug: projectsprojectidcomments-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Comments