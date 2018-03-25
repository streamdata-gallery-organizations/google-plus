---
swagger: "2.0"
info:
  title: Google Plus
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities/{activityId}/comments:
    get:
      summary: Get Activity Comments
      description: List all of the comments for an activity
      operationId: plus.comments.list
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get comments for
      - in: query
        name: maxResults
        description: The maximum number of comments to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: sortOrder
        description: The order in which to sort the list of comments
      responses:
        200:
          description: OK
      tags:
      - comment
definitions: []
x-collection-name: Google Plus
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