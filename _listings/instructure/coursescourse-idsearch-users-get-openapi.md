---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API List users in course
  description: List users in course.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/search_users:
    get:
      summary: List users in course
      description: List users in course.
      operationId: list-users-in-course
      x-api-path-slug: coursescourse-idsearch-users-get
      parameters:
      - in: query
        name: enrollment_role
        description: Deprecated When set, only return users enrolled with the specifiedncourse-level
          role
      - in: query
        name: enrollment_role_id
        description: When set, only return courses where the user is enrolled with
          the specifiedncourse-level role
      - in: query
        name: enrollment_state[]
        description: When set, only return users where the enrollment workflow state
          is of onenof the given types
      - in: query
        name: enrollment_type[]
        description: When set, only return users where the user is enrolled as this
          type
      - in: query
        name: include[]
        description: 'u201cemailu201d: Optional user email'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: user_id
        description: If included, the user will be queried and if the user is part
          of the usersnset, the page parameter will be modified so that the page containingnuser_id
          will be returned
      - in: query
        name: user_ids[]
        description: If included, the course users set will only include users with
          IDsnspecified by the param
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Search
      - Users
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